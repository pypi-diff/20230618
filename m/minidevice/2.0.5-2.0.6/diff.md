# Comparing `tmp/minidevice-2.0.5.tar.gz` & `tmp/minidevice-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-2.0.5.tar", last modified: Sun Jun 18 04:26:33 2023, max compression
+gzip compressed data, was "minidevice-2.0.6.tar", last modified: Sun Jun 18 05:31:15 2023, max compression
```

## Comparing `minidevice-2.0.5.tar` & `minidevice-2.0.6.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 04:26:33.153939 minidevice-2.0.5/
--rw-rw-rw-   0        0        0     2392 2023-06-18 04:26:33.151649 minidevice-2.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2098 2023-06-17 15:02:43.000000 minidevice-2.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 04:26:33.123551 minidevice-2.0.5/minidevice/
--rw-rw-rw-   0        0        0     2758 2023-06-18 04:18:15.000000 minidevice-2.0.5/minidevice/DroidCast.py
--rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.0.5/minidevice/QueueUtils.py
--rw-rw-rw-   0        0        0      226 2023-06-17 14:47:51.000000 minidevice-2.0.5/minidevice/__init__.py
--rw-rw-rw-   0        0        0    21023 2023-06-18 04:23:42.000000 minidevice-2.0.5/minidevice/adb.py
--rw-rw-rw-   0        0        0    20739 2023-06-18 02:48:13.000000 minidevice-2.0.5/minidevice/images.py
--rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.0.5/minidevice/logger.py
--rw-rw-rw-   0        0        0    12808 2023-06-18 04:22:01.000000 minidevice-2.0.5/minidevice/minicap.py
--rw-rw-rw-   0        0        0     1714 2023-06-18 04:22:45.000000 minidevice-2.0.5/minidevice/minitouch.py
--rw-rw-rw-   0        0        0      685 2023-06-18 04:24:38.000000 minidevice-2.0.5/minidevice/screencap.py
--rw-rw-rw-   0        0        0      267 2023-06-17 05:58:10.000000 minidevice-2.0.5/minidevice/touch.py
-drwxrwxrwx   0        0        0        0 2023-06-18 04:26:33.150674 minidevice-2.0.5/minidevice.egg-info/
--rw-rw-rw-   0        0        0     2392 2023-06-18 04:26:32.000000 minidevice-2.0.5/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-06-18 04:26:33.000000 minidevice-2.0.5/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 04:26:32.000000 minidevice-2.0.5/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-18 04:26:32.000000 minidevice-2.0.5/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-18 04:26:32.000000 minidevice-2.0.5/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 04:26:33.153939 minidevice-2.0.5/setup.cfg
--rw-rw-rw-   0        0        0      754 2023-06-18 04:15:42.000000 minidevice-2.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 05:31:15.564545 minidevice-2.0.6/
+-rw-rw-rw-   0        0        0     3077 2023-06-18 05:31:15.563538 minidevice-2.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2783 2023-06-18 05:30:28.000000 minidevice-2.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 05:31:15.530305 minidevice-2.0.6/minidevice/
+-rw-rw-rw-   0        0        0     2758 2023-06-18 04:18:15.000000 minidevice-2.0.6/minidevice/DroidCast.py
+-rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.0.6/minidevice/QueueUtils.py
+-rw-rw-rw-   0        0        0      268 2023-06-18 05:20:44.000000 minidevice-2.0.6/minidevice/__init__.py
+-rw-rw-rw-   0        0        0    21023 2023-06-18 04:23:42.000000 minidevice-2.0.6/minidevice/adb.py
+-rw-rw-rw-   0        0        0     1659 2023-06-18 05:27:30.000000 minidevice-2.0.6/minidevice/device.py
+-rw-rw-rw-   0        0        0    20739 2023-06-18 02:48:13.000000 minidevice-2.0.6/minidevice/images.py
+-rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.0.6/minidevice/logger.py
+-rw-rw-rw-   0        0        0    12808 2023-06-18 04:22:01.000000 minidevice-2.0.6/minidevice/minicap.py
+-rw-rw-rw-   0        0        0     1720 2023-06-18 05:21:56.000000 minidevice-2.0.6/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0      687 2023-06-18 04:29:14.000000 minidevice-2.0.6/minidevice/screencap.py
+-rw-rw-rw-   0        0        0      267 2023-06-17 05:58:10.000000 minidevice-2.0.6/minidevice/touch.py
+drwxrwxrwx   0        0        0        0 2023-06-18 05:31:15.559634 minidevice-2.0.6/minidevice.egg-info/
+-rw-rw-rw-   0        0        0     3077 2023-06-18 05:31:15.000000 minidevice-2.0.6/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-06-18 05:31:15.000000 minidevice-2.0.6/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 05:31:15.000000 minidevice-2.0.6/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-18 05:31:15.000000 minidevice-2.0.6/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-18 05:31:15.000000 minidevice-2.0.6/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 05:31:15.565550 minidevice-2.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      754 2023-06-18 05:31:12.000000 minidevice-2.0.6/setup.py
```

### Comparing `minidevice-2.0.5/README.md` & `minidevice-2.0.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # minidevice v2
-重构代码,添加DroidCast截图方法
+无需关系每个实现方式本身,只需要填入方法即可，未来维护升级添加新方法也只需要在Minidevice中添加新的方法映射即可
 ## minicap/minitouch一键配置
 ### 源码
 [sh脚本](script.sh)
 ### 使用方法
 ```sh
  adb -s ${设备id} shell "curl -o /sdcard/script.sh https://raw.githubusercontent.com/NakanoSanku/minidevice/master/script.sh && sh /sdcard/script.sh"
 ```
@@ -32,14 +32,43 @@
 
 由于uiautomator截图严重拉高模拟器cpu占用
 
 加上uiautomator已许久未更新,移除这一方法
 ## requirements
 `opencv-python` [`pyminitouch`](https://github.com/williamfzc/pyminitouch)
 ## 使用实例
+
+```python
+#操作方法
+TOUCH_METHODS = {
+    "Minitouch": Minitouch,
+     "ADBtouch": ADBtouch
+     }
+```
+```python
+#截图方法
+SCREEN_CAP_METHODS = {
+    "DroidCast": DroidCast,
+     "Minicap": Minicap, 
+     "ADBcap": ADBcap
+     }
+```
+```python
+from minidevice import MiniDevice
+d=MiniDevice(device="127.0.0.1:16834", screen_cap_method="DroidCast", touch_method="Minitouch")
+#截图
+img=d.get_screen()
+#保存截图
+d.save_screen()
+#点击
+d.click(x=100,y=100,duration=100)
+#滑动
+d.swipe([(100,100),(500,500)],duration=300)
+```
+
 采用抽象类定义截图基类
 
 所以[DroidCast](https://github.com/rayworks/DroidCast),[Minicap](https://github.com/DeviceFarmer/minicap),ADBcap使用方法一模一样
 ```python
 from minidevice import Minicap
 #创建截图对象
 capdevice = Minicap("127.0.0.1:16834")
```

### Comparing `minidevice-2.0.5/minidevice/DroidCast.py` & `minidevice-2.0.6/minidevice/DroidCast.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.5/minidevice/QueueUtils.py` & `minidevice-2.0.6/minidevice/QueueUtils.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.5/minidevice/adb.py` & `minidevice-2.0.6/minidevice/adb.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.5/minidevice/images.py` & `minidevice-2.0.6/minidevice/images.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.5/minidevice/minicap.py` & `minidevice-2.0.6/minidevice/minicap.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.5/minidevice/minitouch.py` & `minidevice-2.0.6/minidevice/minitouch.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.abi = self.minitouch_adb.get_abi()
 
     def __minitouch_install(self):
         MNT_HOME = "/data/local/tmp/minitouch"
         self.minitouch_adb.push_file(f"{MINITOUCH_PATH}/{self.abi}/minitouch", MNT_HOME)
         self.minitouch_adb.change_file_permission("+x", MNT_HOME)
 
-    def click(self, x: int, y: int, duration: int):
+    def click(self, x: int, y: int, duration: int = 100):
         """
         click minitouch 点击
 
         Args:
             x (int): 横坐标
             y (int): 纵坐标
             duration (int, optional): 持续时间. Defaults to 100.
```

### Comparing `minidevice-2.0.5/minidevice/screencap.py` & `minidevice-2.0.6/minidevice/screencap.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,8 +16,9 @@
     def save_screencap(self, filename="screencap.png"):
         """
         save_screencap 保存截图
 
         Args:
             filename (str, optional): 截图保存路径. Defaults to "screencap.png".
         """
-        cv2.imencode(ext=".jpg", img=self.screencap_opencv())[1].tofile(filename)
+        with open(filename,"wb") as fp:
+            fp.write(self.screencap_raw())
```

### Comparing `minidevice-2.0.5/setup.py` & `minidevice-2.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='minidevice',
-      version='2.0.5',
+      version='2.0.6',
       description='Android Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku/minidevice',
       license='MIT',
```

