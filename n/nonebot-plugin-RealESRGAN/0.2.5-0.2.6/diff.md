# Comparing `tmp/nonebot_plugin_RealESRGAN-0.2.5.tar.gz` & `tmp/nonebot_plugin_RealESRGAN-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_RealESRGAN-0.2.5.tar", last modified: Tue Jan 31 07:44:32 2023, max compression
+gzip compressed data, was "nonebot_plugin_RealESRGAN-0.2.6.tar", last modified: Sun Jun 18 03:32:45 2023, max compression
```

## Comparing `nonebot_plugin_RealESRGAN-0.2.5.tar` & `nonebot_plugin_RealESRGAN-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-01-31 07:44:32.018016 nonebot_plugin_RealESRGAN-0.2.5/
--rw-rw-rw-   0        0        0     1749 2023-01-31 07:44:31.993016 nonebot_plugin_RealESRGAN-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      701 2023-01-31 07:42:28.000000 nonebot_plugin_RealESRGAN-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-01-31 07:44:31.553647 nonebot_plugin_RealESRGAN-0.2.5/nonebot_plugin_RealESRGAN/
--rw-rw-rw-   0        0        0     2826 2022-10-21 05:53:18.000000 nonebot_plugin_RealESRGAN-0.2.5/nonebot_plugin_RealESRGAN/__init__.py
--rw-rw-rw-   0        0        0      360 2022-10-21 05:59:01.000000 nonebot_plugin_RealESRGAN-0.2.5/nonebot_plugin_RealESRGAN/__version__.py
--rw-rw-rw-   0        0        0     3039 2022-09-23 09:39:06.000000 nonebot_plugin_RealESRGAN-0.2.5/nonebot_plugin_RealESRGAN/utils.py
-drwxrwxrwx   0        0        0        0 2023-01-31 07:44:31.963017 nonebot_plugin_RealESRGAN-0.2.5/nonebot_plugin_RealESRGAN.egg-info/
--rw-rw-rw-   0        0        0     1749 2023-01-31 07:44:31.000000 nonebot_plugin_RealESRGAN-0.2.5/nonebot_plugin_RealESRGAN.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-01-31 07:44:31.000000 nonebot_plugin_RealESRGAN-0.2.5/nonebot_plugin_RealESRGAN.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-31 07:44:31.000000 nonebot_plugin_RealESRGAN-0.2.5/nonebot_plugin_RealESRGAN.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-01-31 07:44:31.000000 nonebot_plugin_RealESRGAN-0.2.5/nonebot_plugin_RealESRGAN.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-01-31 07:44:31.000000 nonebot_plugin_RealESRGAN-0.2.5/nonebot_plugin_RealESRGAN.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-31 07:44:32.018016 nonebot_plugin_RealESRGAN-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     4047 2023-01-31 07:42:47.000000 nonebot_plugin_RealESRGAN-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:32:45.185206 nonebot_plugin_RealESRGAN-0.2.6/
+-rw-rw-rw-   0        0        0     1749 2023-06-18 03:32:45.184206 nonebot_plugin_RealESRGAN-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      701 2023-01-31 07:42:28.000000 nonebot_plugin_RealESRGAN-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 03:32:45.170206 nonebot_plugin_RealESRGAN-0.2.6/nonebot_plugin_RealESRGAN/
+-rw-rw-rw-   0        0        0     2980 2023-06-18 03:31:51.000000 nonebot_plugin_RealESRGAN-0.2.6/nonebot_plugin_RealESRGAN/__init__.py
+-rw-rw-rw-   0        0        0      360 2023-06-18 03:32:30.000000 nonebot_plugin_RealESRGAN-0.2.6/nonebot_plugin_RealESRGAN/__version__.py
+-rw-rw-rw-   0        0        0     3039 2022-09-23 09:39:06.000000 nonebot_plugin_RealESRGAN-0.2.6/nonebot_plugin_RealESRGAN/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:32:45.182207 nonebot_plugin_RealESRGAN-0.2.6/nonebot_plugin_RealESRGAN.egg-info/
+-rw-rw-rw-   0        0        0     1749 2023-06-18 03:32:45.000000 nonebot_plugin_RealESRGAN-0.2.6/nonebot_plugin_RealESRGAN.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-06-18 03:32:45.000000 nonebot_plugin_RealESRGAN-0.2.6/nonebot_plugin_RealESRGAN.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 03:32:45.000000 nonebot_plugin_RealESRGAN-0.2.6/nonebot_plugin_RealESRGAN.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-18 03:32:45.000000 nonebot_plugin_RealESRGAN-0.2.6/nonebot_plugin_RealESRGAN.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-06-18 03:32:45.000000 nonebot_plugin_RealESRGAN-0.2.6/nonebot_plugin_RealESRGAN.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 03:32:45.186207 nonebot_plugin_RealESRGAN-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     4006 2023-06-18 03:32:33.000000 nonebot_plugin_RealESRGAN-0.2.6/setup.py
```

### Comparing `nonebot_plugin_RealESRGAN-0.2.5/PKG-INFO` & `nonebot_plugin_RealESRGAN-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_RealESRGAN
-Version: 0.2.5
+Version: 0.2.6
 Summary: 一个基于nonebot2机器人的对图像进行超分辨率重建插件
 Home-page: https://github.com/staskaer/nonebot_plugin_RealESRGAN
 Author: Staskaer
 Author-email: liujiaxin011121@gmail.com
 License: BSD 3-Clause
 Description: 
         # none_bot_Real-ESRGAN
```

### Comparing `nonebot_plugin_RealESRGAN-0.2.5/README.md` & `nonebot_plugin_RealESRGAN-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_RealESRGAN-0.2.5/nonebot_plugin_RealESRGAN/__init__.py` & `nonebot_plugin_RealESRGAN-0.2.6/nonebot_plugin_RealESRGAN/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,81 @@
 from .utils import *
-from nonebot.adapters.onebot.v11 import Message, MessageEvent, MessageSegment, Bot, Event
+from nonebot.adapters.onebot.v11 import (
+    Message,
+    MessageEvent,
+    MessageSegment,
+    Bot,
+    Event,
+)
 from nonebot.params import T_State, CommandArg
 from nonebot.plugin import on_command
 from nonebot.adapters.onebot.v11.helpers import HandleCancellation
 from json import loads
 from nonebot import get_driver
 
 try:
     api = loads(get_driver().config.json())["realesrgan_api"]
 except:
-    api = 'https://hf.space/embed/ppxxxg22/Real-ESRGAN/api/predict/'
-
+    api = "https://ppxxxg22-real-esrgan.hf.space/api/predict/"
 real_esrgan = on_command(
     "重建", aliases={"real-esrgan", "超分辨率重建", "esrgan", "real_esrgan"}, priority=30
 )
 
 
 @real_esrgan.handle()
 async def real_esrgan_handle_first(
     bot: Bot,
     event: MessageEvent,
     state: T_State,
     args: Message = CommandArg(),
 ):
-    state['id'] = event.get_user_id()
+    state["id"] = event.get_user_id()
     for seg in args:
         if seg.type == "text":
             state["mode"] = seg.data["text"].strip()
         if seg.type == "image":
-            state['img'] = event.message['image']
+            state["img"] = event.message["image"]
             break
 
 
-@real_esrgan.got("mode", prompt="请提供重建模式(二刺螈:anime，其他:base)，模式不绝对，可以任意选", parameterless=[HandleCancellation("已取消")])
+@real_esrgan.got(
+    "mode",
+    prompt="请提供重建模式(二刺螈:anime，其他:base)，模式不绝对，可以任意选",
+    parameterless=[HandleCancellation("已取消")],
+)
 async def real_esrgan_get_mode(event: MessageEvent, state: T_State):
     mode = str(state["mode"]).strip()
     if mode not in ["anime", "base"]:
         await real_esrgan.reject('"base" | "anime", 二选一')
 
 
-@real_esrgan.got("img", prompt="请上传需要超分辨率重建的图片", parameterless=[HandleCancellation("已取消")])
+@real_esrgan.got(
+    "img", prompt="请上传需要超分辨率重建的图片", parameterless=[HandleCancellation("已取消")]
+)
 async def real_esrgan_handle_img(event: MessageEvent, state: T_State):
     # 先拿到需要转换的图
     for seg in state["img"]:
         if seg.type == "image":
             img = await get_img(seg.data["url"])
             break
     else:
         await real_esrgan.finish(Message(f"[CQ:at,qq={state['id']}]不是图捏"))
     # 下面来处理图片
     try:
-        json_data = img_encode_to_json(img, state['mode'])  # 先获取图片并进行编码
+        json_data = img_encode_to_json(img, state["mode"])  # 先获取图片并进行编码
         if json_data is None:
-            await real_esrgan.finish(Message(f"[CQ:at,qq={state['id']}]服务器无法接收到这张图捏,要不重试试试？"))
+            await real_esrgan.finish(
+                Message(f"[CQ:at,qq={state['id']}]服务器无法接收到这张图捏,要不重试试试？")
+            )
         result = await get_result(json_data, api=api)  # 然后进行超分辨率重建
         if result is None:
-            await real_esrgan.finish(Message(f"[CQ:at,qq={state['id']}]这张图没能被正确解析，可能网络连接失败或者是由于远程服务器免费额度耗尽，如果是后者建议联系管理员使用自建仓库(免费)"))
+            await real_esrgan.finish(
+                Message(
+                    f"[CQ:at,qq={state['id']}]这张图没能被正确解析，可能网络连接失败或者是由于远程服务器免费额度耗尽，如果是后者建议联系管理员使用自建仓库(免费)"
+                )
+            )
         img = img_decode_from_json(result)  # 获取重建后图片并进行解码发送
         await real_esrgan.finish(MessageSegment.image(img))
     except Exception as e:
         ...
         # print('错误类型是', e.__class__.__name__)
         # print('错误明细是', e)
```

### Comparing `nonebot_plugin_RealESRGAN-0.2.5/nonebot_plugin_RealESRGAN/utils.py` & `nonebot_plugin_RealESRGAN-0.2.6/nonebot_plugin_RealESRGAN/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_RealESRGAN-0.2.5/nonebot_plugin_RealESRGAN.egg-info/PKG-INFO` & `nonebot_plugin_RealESRGAN-0.2.6/nonebot_plugin_RealESRGAN.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-RealESRGAN
-Version: 0.2.5
+Version: 0.2.6
 Summary: 一个基于nonebot2机器人的对图像进行超分辨率重建插件
 Home-page: https://github.com/staskaer/nonebot_plugin_RealESRGAN
 Author: Staskaer
 Author-email: liujiaxin011121@gmail.com
 License: BSD 3-Clause
 Description: 
         # none_bot_Real-ESRGAN
```

### Comparing `nonebot_plugin_RealESRGAN-0.2.5/setup.py` & `nonebot_plugin_RealESRGAN-0.2.6/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,27 +8,24 @@
 import os
 import sys
 from shutil import rmtree
 
 from setuptools import find_packages, setup, Command
 
 # Package meta-data.
-NAME = 'nonebot_plugin_RealESRGAN'
-DESCRIPTION = '一个基于nonebot2机器人的对图像进行超分辨率重建插件'
-URL = 'https://github.com/staskaer/nonebot_plugin_RealESRGAN'
-EMAIL = 'liujiaxin011121@gmail.com'
-AUTHOR = 'Staskaer'
-REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '0.2.5'
+NAME = "nonebot_plugin_RealESRGAN"
+DESCRIPTION = "一个基于nonebot2机器人的对图像进行超分辨率重建插件"
+URL = "https://github.com/staskaer/nonebot_plugin_RealESRGAN"
+EMAIL = "liujiaxin011121@gmail.com"
+AUTHOR = "Staskaer"
+REQUIRES_PYTHON = ">=3.7.0"
+VERSION = "0.2.6"
 
 # What packages are required for this module to be executed?
-REQUIRED = [
-    'aiohttp',
-    'nonebot-adapter-onebot',
-    'nonebot2']
+REQUIRED = ["aiohttp", "nonebot-adapter-onebot", "nonebot2"]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
@@ -37,98 +34,95 @@
 # If you do change the License, remember to change the Trove Classifier for that!
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import the README and use it as the long-description.
 # Note: this will only work if 'README.md' is present in your MANIFEST.in file!
 try:
-    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
-        long_description = '\n' + f.read()
+    with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
+        long_description = "\n" + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 # Load the package's __version__.py module as a dictionary.
 about = {}
 if not VERSION:
     project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
-    with open(os.path.join(here, project_slug, '__version__.py')) as f:
+    with open(os.path.join(here, project_slug, "__version__.py")) as f:
         exec(f.read(), about)
 else:
-    about['__version__'] = VERSION
+    about["__version__"] = VERSION
 
 
 class UploadCommand(Command):
     """Support setup.py upload."""
 
-    description = 'Build and publish the package.'
+    description = "Build and publish the package."
     user_options = []
 
     @staticmethod
     def status(s):
         """Prints things in bold."""
-        print('\033[1m{0}\033[0m'.format(s))
+        print("\033[1m{0}\033[0m".format(s))
 
     def initialize_options(self):
         pass
 
     def finalize_options(self):
         pass
 
     def run(self):
         try:
-            self.status('Removing previous builds…')
-            rmtree(os.path.join(here, 'dist'))
+            self.status("Removing previous builds…")
+            rmtree(os.path.join(here, "dist"))
         except OSError:
             pass
 
-        self.status('Building Source and Wheel (universal) distribution…')
-        os.system(
-            '{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
-
-        self.status('Uploading the package to PyPI via Twine…')
-        os.system('twine upload dist/*')
-
-        self.status('Pushing git tags…')
-        os.system('git tag v{0}'.format(about['__version__']))
-        os.system('git push --tags')
+        self.status("Building Source and Wheel (universal) distribution…")
+        os.system("{0} setup.py sdist bdist_wheel --universal".format(sys.executable))
+
+        self.status("Uploading the package to PyPI via Twine…")
+        os.system("twine upload dist/*")
+
+        self.status("Pushing git tags…")
+        os.system("git tag v{0}".format(about["__version__"]))
+        os.system("git push --tags")
 
         sys.exit()
 
 
 # Where the magic happens:
 setup(
     name=NAME,
-    version=about['__version__'],
+    version=about["__version__"],
     description=DESCRIPTION,
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
-    packages=find_packages(
-        exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
+    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
     # If your package is a single module, use this instead of 'packages':
     # py_modules=['mypackage'],
-
     # entry_points={
     #     'console_scripts': ['mycli=mymodule:cli'],
     # },
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
-    license='BSD 3-Clause',
+    license="BSD 3-Clause",
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
-        'License :: OSI Approved :: BSD License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Programming Language :: Python :: Implementation :: PyPy'
+        "License :: OSI Approved :: BSD License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Programming Language :: Python :: Implementation :: PyPy",
     ],
     # $ setup.py publish support.
     cmdclass={
-        'upload': UploadCommand,
+        "upload": UploadCommand,
     },
 )
```

