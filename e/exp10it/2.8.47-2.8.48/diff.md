# Comparing `tmp/exp10it-2.8.47.tar.gz` & `tmp/exp10it-2.8.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/exp10it-2.8.47.tar", last modified: Fri Mar  3 07:37:19 2023, max compression
+gzip compressed data, was "dist/exp10it-2.8.48.tar", last modified: Sun Jun 18 16:41:22 2023, max compression
```

## Comparing `exp10it-2.8.47.tar` & `exp10it-2.8.48.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 3xp10it    (502) staff       (20)        0 2023-03-03 07:37:19.530129 exp10it-2.8.47/
--rwxr-xr-x   0 3xp10it    (502) staff       (20)       24 2018-01-31 13:35:11.000000 exp10it-2.8.47/MANIFEST.in
--rw-r--r--   0 3xp10it    (502) staff       (20)      530 2023-03-03 07:37:19.530227 exp10it-2.8.47/PKG-INFO
--rwxr-xr-x   0 3xp10it    (502) staff       (20)      103 2018-01-31 13:35:11.000000 exp10it-2.8.47/README.md
--rwxr-xr-x   0 3xp10it    (502) staff       (20)     1035 2018-01-31 13:35:11.000000 exp10it-2.8.47/README.rst
--rwxr-xr-x   0 3xp10it    (502) staff       (20)    18901 2021-08-28 04:50:51.000000 exp10it-2.8.47/api.md
-drwxr-xr-x   0 3xp10it    (502) staff       (20)        0 2023-03-03 07:37:19.529894 exp10it-2.8.47/exp10it.egg-info/
--rw-r--r--   0 3xp10it    (502) staff       (20)      530 2023-03-03 07:37:19.000000 exp10it-2.8.47/exp10it.egg-info/PKG-INFO
--rw-r--r--   0 3xp10it    (502) staff       (20)      262 2023-03-03 07:37:19.000000 exp10it-2.8.47/exp10it.egg-info/SOURCES.txt
--rw-r--r--   0 3xp10it    (502) staff       (20)        1 2023-03-03 07:37:19.000000 exp10it-2.8.47/exp10it.egg-info/dependency_links.txt
--rw-r--r--   0 3xp10it    (502) staff       (20)      113 2023-03-03 07:37:19.000000 exp10it-2.8.47/exp10it.egg-info/requires.txt
--rw-r--r--   0 3xp10it    (502) staff       (20)       18 2023-03-03 07:37:19.000000 exp10it-2.8.47/exp10it.egg-info/top_level.txt
--rw-r--r--   0 3xp10it    (502) staff       (20)        1 2018-04-20 11:29:26.000000 exp10it-2.8.47/exp10it.egg-info/zip-safe
--rw-r--r--   0 3xp10it    (502) staff       (20)   228232 2023-03-03 06:57:57.000000 exp10it-2.8.47/exp10it.py
--rw-r--r--   0 3xp10it    (502) staff       (20)       59 2023-03-03 07:37:19.530776 exp10it-2.8.47/setup.cfg
--rw-r--r--   0 3xp10it    (502) staff       (20)     3167 2023-03-03 07:35:34.000000 exp10it-2.8.47/setup.py
--rw-r--r--   0 3xp10it    (502) staff       (20)      179 2018-01-31 13:35:11.000000 exp10it-2.8.47/updateapi.py
+drwxr-xr-x   0 3xp10it    (502) staff       (20)        0 2023-06-18 16:41:22.000000 exp10it-2.8.48/
+-rw-r--r--   0 3xp10it    (502) staff       (20)      617 2023-06-18 16:41:22.000000 exp10it-2.8.48/PKG-INFO
+drwxr-xr-x   0 3xp10it    (502) staff       (20)        0 2023-06-18 16:41:22.000000 exp10it-2.8.48/exp10it.egg-info/
+-rw-r--r--   0 3xp10it    (502) staff       (20)      617 2023-06-18 16:41:22.000000 exp10it-2.8.48/exp10it.egg-info/PKG-INFO
+-rw-r--r--   0 3xp10it    (502) staff       (20)        1 2018-04-20 11:29:26.000000 exp10it-2.8.48/exp10it.egg-info/zip-safe
+-rw-r--r--   0 3xp10it    (502) staff       (20)      262 2023-06-18 16:41:22.000000 exp10it-2.8.48/exp10it.egg-info/SOURCES.txt
+-rw-r--r--   0 3xp10it    (502) staff       (20)      113 2023-06-18 16:41:22.000000 exp10it-2.8.48/exp10it.egg-info/requires.txt
+-rw-r--r--   0 3xp10it    (502) staff       (20)       18 2023-06-18 16:41:22.000000 exp10it-2.8.48/exp10it.egg-info/top_level.txt
+-rw-r--r--   0 3xp10it    (502) staff       (20)        1 2023-06-18 16:41:22.000000 exp10it-2.8.48/exp10it.egg-info/dependency_links.txt
+-rwxr-xr-x   0 3xp10it    (502) staff       (20)    18901 2021-08-28 04:50:51.000000 exp10it-2.8.48/api.md
+-rw-r--r--   0 3xp10it    (502) staff       (20)   231943 2023-06-18 16:37:35.000000 exp10it-2.8.48/exp10it.py
+-rwxr-xr-x   0 3xp10it    (502) staff       (20)       24 2018-01-31 13:35:11.000000 exp10it-2.8.48/MANIFEST.in
+-rwxr-xr-x   0 3xp10it    (502) staff       (20)      103 2018-01-31 13:35:11.000000 exp10it-2.8.48/README.md
+-rw-r--r--   0 3xp10it    (502) staff       (20)     3167 2023-06-18 16:37:48.000000 exp10it-2.8.48/setup.py
+-rw-r--r--   0 3xp10it    (502) staff       (20)      179 2018-01-31 13:35:11.000000 exp10it-2.8.48/updateapi.py
+-rw-r--r--   0 3xp10it    (502) staff       (20)       59 2023-06-18 16:41:22.000000 exp10it-2.8.48/setup.cfg
+-rwxr-xr-x   0 3xp10it    (502) staff       (20)     1035 2018-01-31 13:35:11.000000 exp10it-2.8.48/README.rst
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `exp10it-2.8.47/PKG-INFO` & `exp10it-2.8.48/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: exp10it
-Version: 2.8.47
+Version: 2.8.48
 Summary: This is a package about network security
 Home-page: http://3xp10it.cc
 Author: quanyechavshuo
 Author-email: quanyechavshuo@gmail.com
 License: MIT
+Description: ### About
+        
+        exp10it是一个与网络安全相关的模块
+        
+        ### API
+        
+        python3 updateapi.py && cat api.md
+        
 Keywords: network security package
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-
-### About
-
-exp10it是一个与网络安全相关的模块
-
-### API
-
-python3 updateapi.py && cat api.md
```

### Comparing `exp10it-2.8.47/README.rst` & `exp10it-2.8.48/README.rst`

 * *Files identical despite different names*

### Comparing `exp10it-2.8.47/api.md` & `exp10it-2.8.48/api.md`

 * *Files identical despite different names*

### Comparing `exp10it-2.8.47/exp10it.egg-info/PKG-INFO` & `exp10it-2.8.48/exp10it.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: exp10it
-Version: 2.8.47
+Version: 2.8.48
 Summary: This is a package about network security
 Home-page: http://3xp10it.cc
 Author: quanyechavshuo
 Author-email: quanyechavshuo@gmail.com
 License: MIT
+Description: ### About
+        
+        exp10it是一个与网络安全相关的模块
+        
+        ### API
+        
+        python3 updateapi.py && cat api.md
+        
 Keywords: network security package
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-
-### About
-
-exp10it是一个与网络安全相关的模块
-
-### API
-
-python3 updateapi.py && cat api.md
```

### Comparing `exp10it-2.8.47/exp10it.py` & `exp10it-2.8.48/exp10it.py`

 * *Files 1% similar despite different names*

```diff
@@ -2657,14 +2657,80 @@
             if retry_count>=5:
                 print("异常,访问了5次还是没有结果")
                 print("当前请求包是:\n"+string)
                 return None
             time.sleep(3)
             continue
 
+async def async_send_http_packet(string, http_or_https, proxies={},encoding="chardet"):
+    # 发http请求包封装函数,string可以是burpsuite等截包工具中拦截到的包
+    # string要求是burpsuite中抓包抓到的字符串,也即已经经过urlencode
+    # proxy_url为代理地址,eg."http://127.0.0.1:8080"
+    # encoding用于解码服务器返回的内容,默认使用chardet检测出服务器的编码是什么,但有时候chardet检测的不对,这种情况需要手动设置encoding的值
+    # 返回的内容为一个字典,{'code':xxx,'headers':xxx,'html':'xxx'},其中code为int类型,headers是dict类型,html为str类型
+    retry_count=0
+    while True:
+        try:
+            return_value = {'code': 0,'headers': {},'html': ''}
+            string = re.sub(r"^\s", "", string)
+            uri_line = re.search(r"(^.+)", string).group(1)
+            header_dict = {}
+            header_list = re.findall(r"([^:\s]+): ([^\r\n]+)((\n)|(\r\n))", string)
+            for each in header_list:
+                header_dict[each[0]] = each[1]
+            url = http_or_https + "://" + re.search(r"Host: (\S+)", string, re.I).group(
+                1) + re.search(r" (\S+)", uri_line, re.I).group(1)
+            if string[:3] == "GET":
+                if proxies == {}:
+                    async with aiohttp.ClientSession() as session:
+                        async with session.get(url, headers=header_dict, timeout=30, ssl=False) as res:
+                            code = res.status
+                            headers = res.headers
+                            content = await res.text()
+                else:
+                    async with aiohttp.ClientSession() as session:
+                        async with session.get(url, headers=header_dict, proxy=proxies, timeout=30, ssl=False) as res:
+                            code = res.status
+                            headers = res.headers
+                            content = await res.text()
+            elif string[:4] == "POST":
+                post_string = re.search(r"((\r\n\r\n)|(\n\n))(.*)", string).group(4)
+                post_string_bytes = post_string.encode("utf8")
+                if proxies == {}:
+                    async with aiohttp.ClientSession() as session:
+                        async with session.post(url, headers=header_dict, data=post_string_bytes, timeout=30, ssl=False) as res:
+                            code = res.status
+                            headers = res.headers
+                            content = await res.text()
+                else:
+                    async with aiohttp.ClientSession() as session:
+                        async with session.post(url, headers=header_dict, data=post_string_bytes, proxy=proxies, timeout=30, ssl=False) as res:
+                            code = res.status
+                            headers = res.headers
+                            content = await res.text()
+            if encoding=='chardet':
+                import chardet
+                bytes_encoding = chardet.detect(content)['encoding']
+                if bytes_encoding is None:
+                    bytes_encoding="utf8"
+            else:
+                bytes_encoding=encoding
+            content = content.decode(encoding=bytes_encoding, errors="ignore")
+            return_value['code'] = code
+            return_value['headers'] = headers
+            return_value['html'] = content
+            return return_value
+        except:
+            retry_count+=1
+            if retry_count>=5:
+                print("异常,访问了5次还是没有结果")
+                print("当前请求包是:\n"+string)
+                return None
+            time.sleep(3)
+            continue
 
 def set_string_to_clipboard(string):
     import pyperclip
     pyperclip.copy(string)
     if string!=pyperclip.paste():
         pyperclip.copy(string)
```

### Comparing `exp10it-2.8.47/setup.py` & `exp10it-2.8.48/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 DESCRIPTION = "This is a package about network security"
 LONG_DESCRIPTION = read("README.md")
 KEYWORDS = "network security package"
 AUTHOR = "quanyechavshuo"
 AUTHOR_EMAIL = "quanyechavshuo@gmail.com"
 URL = "http://3xp10it.cc"
 
-VERSION = "2.8.47"
+VERSION = "2.8.48"
 LICENSE = "MIT"
 #beepy在linux下可能会安装失败,有需要的情况下要手动安装
 require_package_list=['mechanicalsoup', 'bs4', 'selenium', 'colorama', 'requests', 'configparser', 'chardet', 'wget', 'pymysql','pyperclip','html2text']
 system=platform.system()
 if system in ['Windows','Darwin']:
     #require_package_list.append("beepy")
     try:
```

