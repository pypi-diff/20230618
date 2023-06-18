# Comparing `tmp/pydatawork-0.0.7.tar.gz` & `tmp/pydatawork-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.0.7.tar", last modified: Sun Jun 18 09:14:25 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.0.8.tar", last modified: Sun Jun 18 09:37:57 2023, max compression
```

## Comparing `pydatawork-0.0.7.tar` & `pydatawork-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 09:14:25.000000 pydatawork-0.0.7/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1699 2023-06-18 09:14:25.000000 pydatawork-0.0.7/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      855 2023-06-18 09:13:53.000000 pydatawork-0.0.7/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 09:14:25.000000 pydatawork-0.0.7/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1699 2023-06-18 09:14:25.000000 pydatawork-0.0.7/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-18 09:14:25.000000 pydatawork-0.0.7/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-18 09:14:25.000000 pydatawork-0.0.7/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-18 09:14:25.000000 pydatawork-0.0.7/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     7054 2023-06-18 09:09:22.000000 pydatawork-0.0.7/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-18 09:14:25.000000 pydatawork-0.0.7/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-18 09:10:31.000000 pydatawork-0.0.7/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 09:37:57.000000 pydatawork-0.0.8/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1699 2023-06-18 09:37:57.000000 pydatawork-0.0.8/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      855 2023-06-18 09:13:53.000000 pydatawork-0.0.8/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-18 09:37:57.000000 pydatawork-0.0.8/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1699 2023-06-18 09:37:57.000000 pydatawork-0.0.8/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-18 09:37:57.000000 pydatawork-0.0.8/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-18 09:37:57.000000 pydatawork-0.0.8/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-18 09:37:57.000000 pydatawork-0.0.8/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     6829 2023-06-18 09:36:38.000000 pydatawork-0.0.8/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-18 09:37:57.000000 pydatawork-0.0.8/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-18 09:37:40.000000 pydatawork-0.0.8/setup.py
```

### Comparing `pydatawork-0.0.7/PKG-INFO` & `pydatawork-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.0.7
+Version: 0.0.8
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description:
```

### Comparing `pydatawork-0.0.7/README.md` & `pydatawork-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pydatawork-0.0.7/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.0.8/pydatawork.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.0.7
+Version: 0.0.8
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description:
```

### Comparing `pydatawork-0.0.7/pydatawork.py` & `pydatawork-0.0.8/pydatawork.py`

 * *Files 7% similar despite different names*

```diff
@@ -140,23 +140,17 @@
                 else:
                     break
             except Exception as e:
                 print(e)
                 i += 1  # 添加这一行
                 pass
 
+    if os.path.isdir(os.path.join(path,weibo_name)):
+        pass
+    else:
+        os.mkdir(os.path.join(path,weibo_name))
+    file = os.path.join(path, weibo_name, weibo_name + ".txt")
 
-    if __name__ == "__main__":
-        # if os.path.isdir(path + weibo_name):
-        #     pass
-        # else:
-        #     os.mkdir(path + weibo_name)
-        # file = path + weibo_name + '\\' + weibo_name + ".txt" # 原始代码
-        if os.path.isdir(os.path.join(path,weibo_name)):
-            pass
-        else:
-            os.mkdir(os.path.join(path,weibo_name))
-        file = os.path.join(path, weibo_name, weibo_name + ".txt")
-
-        get_userInfo(id)
-        get_weibo(id, file)
+    get_userInfo(id)
+    get_weibo(id, file)
+    print("微博数据获取完毕")
```

### Comparing `pydatawork-0.0.7/setup.py` & `pydatawork-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.0.7',
+    version='0.0.8',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

