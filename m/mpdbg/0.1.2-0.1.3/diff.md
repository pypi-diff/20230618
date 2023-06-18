# Comparing `tmp/mpdbg-0.1.2.tar.gz` & `tmp/mpdbg-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpdbg-0.1.2.tar", max compression
+gzip compressed data, was "mpdbg-0.1.3.tar", max compression
```

## Comparing `mpdbg-0.1.2.tar` & `mpdbg-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     2655 2023-06-05 01:11:22.161764 mpdbg-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-26 13:12:10.539829 mpdbg-0.1.2/mpdbg/__init__.py
--rw-r--r--   0        0        0       62 2023-05-26 13:44:32.156382 mpdbg-0.1.2/mpdbg/__main__.py
--rw-r--r--   0        0        0     1696 2023-06-05 01:54:52.511760 mpdbg-0.1.2/mpdbg/image.py
--rw-r--r--   0        0        0     4986 2023-06-05 09:51:57.878383 mpdbg-0.1.2/mpdbg/main.py
--rw-r--r--   0        0        0     1435 2023-06-02 01:31:26.251691 mpdbg-0.1.2/mpdbg/mpd_utils.py
--rw-r--r--   0        0        0     1047 2023-05-29 13:15:42.437509 mpdbg-0.1.2/mpdbg/wallpaper.py
--rw-r--r--   0        0        0      573 2023-06-05 09:56:28.838383 mpdbg-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3540 1970-01-01 00:00:00.000000 mpdbg-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2861 2023-06-06 14:06:41.568338 mpdbg-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-06 23:12:34.018429 mpdbg-0.1.3/mpdbg/__init__.py
+-rw-r--r--   0        0        0       62 2023-06-06 23:12:34.025096 mpdbg-0.1.3/mpdbg/__main__.py
+-rw-r--r--   0        0        0     2305 2023-06-09 03:35:25.334558 mpdbg-0.1.3/mpdbg/image.py
+-rw-r--r--   0        0        0     2217 2023-06-08 17:57:09.047878 mpdbg-0.1.3/mpdbg/main.py
+-rw-r--r--   0        0        0     3003 2023-06-09 06:31:43.464544 mpdbg-0.1.3/mpdbg/mpd_utils.py
+-rw-r--r--   0        0        0     5856 2023-06-11 09:46:11.658638 mpdbg-0.1.3/mpdbg/mpdbg.py
+-rw-r--r--   0        0        0      158 2023-06-18 01:50:45.695068 mpdbg-0.1.3/mpdbg/shell.py
+-rw-r--r--   0        0        0     2098 2023-06-18 01:52:31.241730 mpdbg-0.1.3/mpdbg/wallpaper.py
+-rw-r--r--   0        0        0      692 2023-06-18 04:19:03.505781 mpdbg-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3736 1970-01-01 00:00:00.000000 mpdbg-0.1.3/PKG-INFO
```

### Comparing `mpdbg-0.1.2/README.md` & `mpdbg-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -57,7 +57,10 @@
 
 Example for using *mpdbg* with [swww](https://github.com/Horus645/swww) wallpaper setter:
 
     mpdbg run -w ~/wallpaper.png -s 'swww img --transition-type center $image' -e blur
 
 The command above would use *~/wallpaper.png* as wallpaper and *swww* as wallpaper setter. The wallpaper would also be blurred when displaying a cover art image on top of it.
 
+Example for Windows CMD prompt using [WallpaperChanger](https://github.com/philhansen/WallpaperChanger) as wallpaper setter:
+
+    mpdbg run -w C:\wallpaper.png -s "C:\WallpaperChanger.exe $image 4" -e blur
```

### Comparing `mpdbg-0.1.2/mpdbg/image.py` & `mpdbg-0.1.3/mpdbg/image.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,46 @@
-import io
 import logging
 import time
 
+import PIL
 from PIL import Image, ImageOps, ImageFilter
 
 
+class CreateWallpaperException(Exception):
+    """Creating wallpaper image failed"""
+
+
+
 def create_wallpaper_image(
-        wallpaper_path: str, cover_data: bytes, blur: bool = False, grayscale: bool = False, image_format: str = "jpeg",
+        wallpaper_path: str, cover: Image, blur: bool = False, grayscale: bool = False,
         cover_border_size: int = 10, cover_relative_size: float = 0.75, wallpaper_blur_radius: int = 20
-) -> bytes:
+) -> Image:
+    """
+    Create wallpaper image by drawing cover image on top of wallpaper image.
+    :param wallpaper_path: wallpaper file path
+    :param cover_data: encoded image data
+    :param blur: blur background image
+    :param grayscale: convert background image to grayscale
+    :param cover_border_size: how thick border to draw
+    :param cover_relative_size: size of the cover
+    :param wallpaper_blur_radius: blur radius
+    :return: resulting wallpaper image
+    :raise CreateWallpaperException: creating the image failed
+    """
     logger = logging.getLogger("mpdbg")
 
     start_time = time.perf_counter_ns()
 
-    with open(wallpaper_path, "rb") as f:
-        wallpaper = Image.open(f).convert("RGB")
+    try:
+        with open(wallpaper_path, "rb") as file:
+            wallpaper = Image.open(file).convert("RGB")
+    except (FileNotFoundError, PIL.UnidentifiedImageError) as err:
+        raise CreateWallpaperException(f"Failed to open image file {wallpaper_path}: {err}") from err
 
-    cover = Image.open(io.BytesIO(cover_data)).convert("RGB")
+    cover = cover.convert("RGB")
 
     # resize cover
     cover_scale = min(
         wallpaper.width / cover.width * cover_relative_size,
         wallpaper.height / cover.height * cover_relative_size,
     )
     cover = cover.resize(
@@ -35,20 +55,15 @@
         wallpaper = ImageOps.grayscale(wallpaper).convert("RGB")
 
     if blur:
         # blur wallpaper
         wallpaper = wallpaper.filter(ImageFilter.GaussianBlur(radius=wallpaper_blur_radius))
 
     # draw cover on wallpaper
-    x = (wallpaper.width - cover.width) // 2
-    y = (wallpaper.height - cover.height) // 2
-    wallpaper.paste(cover, (x, y))
-
-    # get image data
-    wallpaper_bytes = io.BytesIO()
-    wallpaper.save(wallpaper_bytes, image_format)
-    wallpaper_data = wallpaper_bytes.getvalue()
+    x_pos = (wallpaper.width - cover.width) // 2
+    y_pos = (wallpaper.height - cover.height) // 2
+    wallpaper.paste(cover, (x_pos, y_pos))
 
     time_taken = time.perf_counter_ns() - start_time
     logger.debug("creating wallpaper image took %.3f seconds", time_taken / 1000 / 1000 / 1000)
 
-    return wallpaper_data
+    return wallpaper
```

### Comparing `mpdbg-0.1.2/pyproject.toml` & `mpdbg-0.1.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 [tool.poetry]
 name = "mpdbg"
-version = "0.1.2"
+version = "0.1.3"
 description = "Display MPD's current song's cover art on top of wallpaper"
 authors = ["dragonwit <dragonwit@dragonwit.dev>"]
 readme = "README.md"
 license = "GPL-3.0-only"
 homepage = "https://git.dragonwit.dev/dragonwit/mpdbg-py"
 repository = "https://git.dragonwit.dev/dragonwit/mpdbg-py"
 
 [tool.poetry.dependencies]
-python = ">=3.7"
+python = ">=3.7.2"
 python-mpd2 = "^3.1.0"
 click = "^8.1.3"
 pillow = "^9.5.0"
+mslex = "^1.1.0"
 
 [tool.poetry.scripts]
 mpdbg = "mpdbg.main:main"
 
+[tool.poetry.group.test.dependencies]
+pytest = "^7.3.1"
+pytest-mock = "^3.10.0"
+pylint = "^2.17.4"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mpdbg-0.1.2/PKG-INFO` & `mpdbg-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: mpdbg
-Version: 0.1.2
+Version: 0.1.3
 Summary: Display MPD's current song's cover art on top of wallpaper
 Home-page: https://git.dragonwit.dev/dragonwit/mpdbg-py
 License: GPL-3.0-only
 Author: dragonwit
 Author-email: dragonwit@dragonwit.dev
-Requires-Python: >=3.7
+Requires-Python: >=3.7.2
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: mslex (>=1.1.0,<2.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: python-mpd2 (>=3.1.0,<4.0.0)
 Project-URL: Repository, https://git.dragonwit.dev/dragonwit/mpdbg-py
 Description-Content-Type: text/markdown
 
 # mpdbg
 
@@ -79,8 +79,11 @@
 
 Example for using *mpdbg* with [swww](https://github.com/Horus645/swww) wallpaper setter:
 
     mpdbg run -w ~/wallpaper.png -s 'swww img --transition-type center $image' -e blur
 
 The command above would use *~/wallpaper.png* as wallpaper and *swww* as wallpaper setter. The wallpaper would also be blurred when displaying a cover art image on top of it.
 
+Example for Windows CMD prompt using [WallpaperChanger](https://github.com/philhansen/WallpaperChanger) as wallpaper setter:
+
+    mpdbg run -w C:\wallpaper.png -s "C:\WallpaperChanger.exe $image 4" -e blur
```

