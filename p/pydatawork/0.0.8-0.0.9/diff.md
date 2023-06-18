# Comparing `tmp/pydatawork-0.0.8.tar.gz` & `tmp/pydatawork-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.0.8.tar", last modified: Sun Jun 18 09:37:57 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.0.9.tar", last modified: Sun Jun 18 09:50:57 2023, max compression
```

## Comparing `pydatawork-0.0.8.tar` & `pydatawork-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 09:37:57.000000 pydatawork-0.0.8/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1699 2023-06-18 09:37:57.000000 pydatawork-0.0.8/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      855 2023-06-18 09:13:53.000000 pydatawork-0.0.8/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 09:37:57.000000 pydatawork-0.0.8/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1699 2023-06-18 09:37:57.000000 pydatawork-0.0.8/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-18 09:37:57.000000 pydatawork-0.0.8/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-18 09:37:57.000000 pydatawork-0.0.8/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-18 09:37:57.000000 pydatawork-0.0.8/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     6829 2023-06-18 09:36:38.000000 pydatawork-0.0.8/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-18 09:37:57.000000 pydatawork-0.0.8/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-18 09:37:40.000000 pydatawork-0.0.8/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 09:50:57.000000 pydatawork-0.0.9/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1699 2023-06-18 09:50:57.000000 pydatawork-0.0.9/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      855 2023-06-18 09:13:53.000000 pydatawork-0.0.9/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 09:50:57.000000 pydatawork-0.0.9/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1699 2023-06-18 09:50:57.000000 pydatawork-0.0.9/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-18 09:50:57.000000 pydatawork-0.0.9/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-18 09:50:57.000000 pydatawork-0.0.9/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-18 09:50:57.000000 pydatawork-0.0.9/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     7028 2023-06-18 09:50:17.000000 pydatawork-0.0.9/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-18 09:50:57.000000 pydatawork-0.0.9/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-18 09:50:35.000000 pydatawork-0.0.9/setup.py
```

### Comparing `pydatawork-0.0.8/PKG-INFO` & `pydatawork-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.0.8
+Version: 0.0.9
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description:
```

### Comparing `pydatawork-0.0.8/README.md` & `pydatawork-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pydatawork-0.0.8/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.0.9/pydatawork.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.0.8
+Version: 0.0.9
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description:
```

### Comparing `pydatawork-0.0.8/pydatawork.py` & `pydatawork-0.0.9/pydatawork.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,15 +50,14 @@
     id:微博id；
     weibi_name:存放文件夹的名字。
     """
     path = path
     id = id # 在微博上获取
 
     proxy_addr = "122.241.72.191:808"
-    pic_num = 0
     weibo_name = weibo_name # 可以自定义名字
 
 
     def use_proxy(url, proxy_addr):
         req = urllib.request.Request(url)
         req.add_header("User-Agent",
                     "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/49.0.2623.221 Safari/537.36 SE 2.X MetaSr 1.0")
@@ -92,14 +91,15 @@
         gender = content.get('userInfo').get('gender')
         urank = content.get('userInfo').get('urank')
         print("微博昵称：" + name + "\n" + "微博主页地址：" + profile_url + "\n" + "微博头像地址：" + profile_image_url + "\n" + "是否认证：" + str(verified) + "\n" + "微博说明：" + description + "\n" + "关注人数：" + str(guanzhu) + "\n" + "粉丝数：" + str(fensi) + "\n" + "性别：" + gender + "\n" + "微博等级：" + str(urank) + "\n")
 
 
     def get_weibo(id, file):
         global pic_num
+        pic_num = 0
         i = 1
         while True:
             url = 'https://m.weibo.cn/api/container/getIndex?type=uid&value=' + id
             weibo_url = 'https://m.weibo.cn/api/container/getIndex?type=uid&value=' + id + '&containerid=' + get_containerid(url) + '&page=' + str(i)
             try:
                 data = use_proxy(weibo_url, proxy_addr)
                 content = json.loads(data).get('data')
@@ -140,14 +140,20 @@
                 else:
                     break
             except Exception as e:
                 print(e)
                 i += 1  # 添加这一行
                 pass
 
+    # # 在指定路径下，先建立一个名为weibo的文件夹
+    # if os.path.isdir(os.path.join(path,"weibo")):
+    #     pass
+    # else:
+    #     os.mkdir(os.path.join(path,"weibo"))
+
     if os.path.isdir(os.path.join(path,weibo_name)):
         pass
     else:
         os.mkdir(os.path.join(path,weibo_name))
     file = os.path.join(path, weibo_name, weibo_name + ".txt")
 
     get_userInfo(id)
```

### Comparing `pydatawork-0.0.8/setup.py` & `pydatawork-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.0.8',
+    version='0.0.9',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

