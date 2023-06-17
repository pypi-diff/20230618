# Comparing `tmp/y2mate-api-0.0.2.tar.gz` & `tmp/y2mate-api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "y2mate-api-0.0.2.tar", last modified: Sat Jun 17 14:49:57 2023, max compression
+gzip compressed data, was "y2mate-api-0.0.3.tar", last modified: Sat Jun 17 22:05:25 2023, max compression
```

## Comparing `y2mate-api-0.0.2.tar` & `y2mate-api-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-17 14:49:57.556150 y2mate-api-0.0.2/
--rw-rw----   0 root         (0) everybody  (9997)     1064 2023-06-16 15:42:28.000000 y2mate-api-0.0.2/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)    10336 2023-06-17 14:49:57.536150 y2mate-api-0.0.2/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     9241 2023-06-17 14:49:23.000000 y2mate-api-0.0.2/README.md
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-17 14:49:57.556150 y2mate-api-0.0.2/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1513 2023-06-17 13:25:23.000000 y2mate-api-0.0.2/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-17 14:49:57.052150 y2mate-api-0.0.2/tests/
--rw-rw----   0 root         (0) everybody  (9997)      255 2023-06-15 19:45:34.000000 y2mate-api-0.0.2/tests/test.py
--rw-rw----   0 root         (0) everybody  (9997)      267 2023-06-15 19:39:07.000000 y2mate-api-0.0.2/tests/test_1.py
--rw-rw----   0 root         (0) everybody  (9997)      261 2023-06-15 20:21:38.000000 y2mate-api-0.0.2/tests/test_3.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-17 14:49:57.236150 y2mate-api-0.0.2/y2mate_api/
--rw-rw----   0 root         (0) everybody  (9997)      490 2023-06-17 14:45:18.000000 y2mate-api-0.0.2/y2mate_api/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     4631 2023-06-17 13:45:27.000000 y2mate-api-0.0.2/y2mate_api/console.py
--rw-rw----   0 root         (0) everybody  (9997)    11174 2023-06-17 14:14:13.000000 y2mate-api-0.0.2/y2mate_api/downloader.py
--rw-rw----   0 root         (0) everybody  (9997)    14661 2023-06-17 14:38:29.000000 y2mate-api-0.0.2/y2mate_api/main.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-17 14:49:57.512150 y2mate-api-0.0.2/y2mate_api.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)    10336 2023-06-17 14:49:55.000000 y2mate-api-0.0.2/y2mate_api.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      367 2023-06-17 14:49:56.000000 y2mate-api-0.0.2/y2mate_api.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-17 14:49:55.000000 y2mate-api-0.0.2/y2mate_api.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       51 2023-06-17 14:49:55.000000 y2mate-api-0.0.2/y2mate_api.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       74 2023-06-17 14:49:55.000000 y2mate-api-0.0.2/y2mate_api.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)       11 2023-06-17 14:49:55.000000 y2mate-api-0.0.2/y2mate_api.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-17 22:05:25.679842 y2mate-api-0.0.3/
+-rw-rw----   0 root         (0) everybody  (9997)     1064 2023-06-16 15:42:28.000000 y2mate-api-0.0.3/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)    10355 2023-06-17 22:05:25.663842 y2mate-api-0.0.3/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     9260 2023-06-17 22:05:02.000000 y2mate-api-0.0.3/README.md
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-17 22:05:25.679842 y2mate-api-0.0.3/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1535 2023-06-17 16:53:45.000000 y2mate-api-0.0.3/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-17 22:05:25.283842 y2mate-api-0.0.3/tests/
+-rw-rw----   0 root         (0) everybody  (9997)      255 2023-06-15 19:45:34.000000 y2mate-api-0.0.3/tests/test.py
+-rw-rw----   0 root         (0) everybody  (9997)      267 2023-06-15 19:39:07.000000 y2mate-api-0.0.3/tests/test_1.py
+-rw-rw----   0 root         (0) everybody  (9997)      261 2023-06-15 20:21:38.000000 y2mate-api-0.0.3/tests/test_3.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-17 22:05:25.399842 y2mate-api-0.0.3/y2mate_api/
+-rw-rw----   0 root         (0) everybody  (9997)      490 2023-06-17 16:27:02.000000 y2mate-api-0.0.3/y2mate_api/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     5072 2023-06-17 18:18:06.000000 y2mate-api-0.0.3/y2mate_api/console.py
+-rw-rw----   0 root         (0) everybody  (9997)    13244 2023-06-17 21:46:43.000000 y2mate-api-0.0.3/y2mate_api/downloader.py
+-rw-rw----   0 root         (0) everybody  (9997)    14839 2023-06-17 19:43:50.000000 y2mate-api-0.0.3/y2mate_api/main.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-17 22:05:25.643842 y2mate-api-0.0.3/y2mate_api.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)    10355 2023-06-17 22:05:24.000000 y2mate-api-0.0.3/y2mate_api.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      367 2023-06-17 22:05:24.000000 y2mate-api-0.0.3/y2mate_api.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-17 22:05:24.000000 y2mate-api-0.0.3/y2mate_api.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       51 2023-06-17 22:05:24.000000 y2mate-api-0.0.3/y2mate_api.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       85 2023-06-17 22:05:24.000000 y2mate-api-0.0.3/y2mate_api.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)       11 2023-06-17 22:05:24.000000 y2mate-api-0.0.3/y2mate_api.egg-info/top_level.txt
```

### Comparing `y2mate-api-0.0.2/LICENSE` & `y2mate-api-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.2/PKG-INFO` & `y2mate-api-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y2mate-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: Download youtube videos and audios by title or link
 Home-page: https://github.com/Simatwa/y2mate-api
 Author: Smartwa
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/y2mate-api/issues/new
@@ -27,15 +27,15 @@
 License-File: LICENSE
 
 # y2mate-api
 
 <p align="center">
 <a href="https://github.com/Simatwa/y2mate-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.2&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.3&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
 
@@ -188,65 +188,61 @@
 </summary>
 
 ```
 usage: y2mate [-h] [-v] [-f mp4|mp3]
               [-q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
               [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]]
               [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
-              [-t TIMEOUT] [-i PATH] [--disable-bar]
-              [--ask] [--unique] [--history]
-              [--clear]
+              [-t TIMEOUT] [-i PATH] [-thr THREAD]
+              [--disable-bar] [--ask] [--unique] [--quiet]
+              [--history] [--clear]
               [query ...]
 
 Download youtube videos and audios by title or link
 
 positional arguments:
-  query                 Youtube video title, link or
-                        id - None
+  query                 Youtube video title, link or id - None
 
 options:
-  -h, --help            show this help message and
-                        exit
-  -v, --version         show program's version number
-                        and exit
+  -h, --help            show this help message and exit
+  -v, --version         show program's version number and exit
   -f mp4|mp3, --format mp4|mp3
-                        Specify media type -
-                        audio/video
+                        Specify media type - audio/video
   -q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps, --quality 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps
                         Media quality -720p
   -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3
-                        Other media formats incase of
-                        multiple options - mp4/mp3
+                        Other media formats incase of multiple
+                        options - mp4/mp3
   -k [KEYWORD ...], --keyword [KEYWORD ...]
-                        Media should contain this
-                        keywords - None
+                        Media should contain this keywords -
+                        None
   -a [AUTHOR ...], --author [AUTHOR ...]
-                        Media author i.e YouTube
-                        channel name - None
+                        Media author i.e YouTube channel name -
+                        None
   -l LIMIT, --limit LIMIT
-                        Total videos to be downloaded
-                        - 1
-  -d PATH, --dir PATH   Directory for saving the
-                        contents - /storage/emulated/
-                        0/git/Smartwa/y2mate-api
+                        Total videos to be downloaded - 1
+  -d PATH, --dir PATH   Directory for saving the contents -
+                        /storage/emulated/0/git/Smartwa
   -t TIMEOUT, --timeout TIMEOUT
                         Http request timeout - 30s
   -i PATH, --input PATH
-                        Path to text file containing
-                        query per line - None
-  --disable-bar         Disables download progress
-                        bar - False
-  --ask                 Confirm before downloading
-                        file - False
-  --unique              Auto-skip any media that you
-                        once dowloaded - False
-  --history             Stdout all media metadata
-                        ever downloaded - False
-  --clear               Clear all download histories
-                        - False
+                        Path to text file containing query per
+                        line - None
+  -thr THREAD, --thread THREAD
+                        Download [x] amount of videos/audios at
+                        once - 1
+  --disable-bar         Disables download progress bar - False
+  --ask                 Confirm before downloading file - False
+  --unique              Auto-skip any media that you once
+                        dowloaded - False
+  --quiet               Not to stdout anything other than logs -
+                        False
+  --history             Stdout all media metadata ever
+                        downloaded - False
+  --clear               Clear all download histories - False
 
 This script has no official relation with y2mate.com
 ```
 </details>
 
 - Review [CHANGELOG](https://github.com/Simatwa/y2mate-api/blob/main/Docs/CHANGELOG.md) for latest updates.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.2 Summary: Download youtube
+Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.3 Summary: Download youtube
 videos and audios by title or link Home-page: https://github.com/Simatwa/
 y2mate-api Author: Smartwa Author-email: smartwacaleb@gmail.com Maintainer:
 Smartwa License: MIT Project-URL: Bug Report, https://github.com/Simatwa/
 y2mate-api/issues/new Keywords: y2mate,videos,video-api,youtube Classifier:
 License :: OSI Approved :: MIT License Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: Free For Home Use Classifier: Intended
@@ -66,34 +66,37 @@
 `Handler.run` * progress_bar : Stdout media-name & Display progress bar -
 `Handler.save` * third_dict : Response of `third_query.run()` * dir : Directory
 for saving the contents * progress_bar : Stdout media-name & Display download
 progress bar    For more info run `$ y2mate -h`  ``` usage: y2mate [-h] [-v] [-
 f mp4|mp3] [-
 q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
 [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]] [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
-[-t TIMEOUT] [-i PATH] [--disable-bar] [--ask] [--unique] [--history] [--clear]
-[query ...] Download youtube videos and audios by title or link positional
-arguments: query Youtube video title, link or id - None options: -h, --help
-show this help message and exit -v, --version show program's version number and
-exit -f mp4|mp3, --format mp4|mp3 Specify media type - audio/video -
+[-t TIMEOUT] [-i PATH] [-thr THREAD] [--disable-bar] [--ask] [--unique] [--
+quiet] [--history] [--clear] [query ...] Download youtube videos and audios by
+title or link positional arguments: query Youtube video title, link or id -
+None options: -h, --help show this help message and exit -v, --version show
+program's version number and exit -f mp4|mp3, --format mp4|mp3 Specify media
+type - audio/video -
 q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps,
 --quality
 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps
 Media quality -720p -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3 Other media
 formats incase of multiple options - mp4/mp3 -k [KEYWORD ...], --keyword
 [KEYWORD ...] Media should contain this keywords - None -a [AUTHOR ...], --
 author [AUTHOR ...] Media author i.e YouTube channel name - None -l LIMIT, --
 limit LIMIT Total videos to be downloaded - 1 -d PATH, --dir PATH Directory for
-saving the contents - /storage/emulated/ 0/git/Smartwa/y2mate-api -t TIMEOUT, -
--timeout TIMEOUT Http request timeout - 30s -i PATH, --input PATH Path to text
-file containing query per line - None --disable-bar Disables download progress
+saving the contents - /storage/emulated/0/git/Smartwa -t TIMEOUT, --timeout
+TIMEOUT Http request timeout - 30s -i PATH, --input PATH Path to text file
+containing query per line - None -thr THREAD, --thread THREAD Download [x]
+amount of videos/audios at once - 1 --disable-bar Disables download progress
 bar - False --ask Confirm before downloading file - False --unique Auto-skip
-any media that you once dowloaded - False --history Stdout all media metadata
-ever downloaded - False --clear Clear all download histories - False This
-script has no official relation with y2mate.com ```  - Review [CHANGELOG]
-(https://github.com/Simatwa/y2mate-api/blob/main/Docs/CHANGELOG.md) for latest
-updates. ## Disclaimer This repository is intended for educational and personal
-use only. The use of this repository for any commercial or illegal purposes is
-strictly prohibited. The repository owner does not endorse or encourage the
-downloading or sharing of copyrighted material without permission. The
-repository owner is not responsible for any misuse of the software or any legal
-consequences that may arise from such misuse.
+any media that you once dowloaded - False --quiet Not to stdout anything other
+than logs - False --history Stdout all media metadata ever downloaded - False -
+-clear Clear all download histories - False This script has no official
+relation with y2mate.com ```  - Review [CHANGELOG](https://github.com/Simatwa/
+y2mate-api/blob/main/Docs/CHANGELOG.md) for latest updates. ## Disclaimer This
+repository is intended for educational and personal use only. The use of this
+repository for any commercial or illegal purposes is strictly prohibited. The
+repository owner does not endorse or encourage the downloading or sharing of
+copyrighted material without permission. The repository owner is not
+responsible for any misuse of the software or any legal consequences that may
+arise from such misuse.
```

### Comparing `y2mate-api-0.0.2/README.md` & `y2mate-api-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # y2mate-api
 
 <p align="center">
 <a href="https://github.com/Simatwa/y2mate-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.2&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.3&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
 
@@ -160,65 +160,61 @@
 </summary>
 
 ```
 usage: y2mate [-h] [-v] [-f mp4|mp3]
               [-q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
               [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]]
               [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
-              [-t TIMEOUT] [-i PATH] [--disable-bar]
-              [--ask] [--unique] [--history]
-              [--clear]
+              [-t TIMEOUT] [-i PATH] [-thr THREAD]
+              [--disable-bar] [--ask] [--unique] [--quiet]
+              [--history] [--clear]
               [query ...]
 
 Download youtube videos and audios by title or link
 
 positional arguments:
-  query                 Youtube video title, link or
-                        id - None
+  query                 Youtube video title, link or id - None
 
 options:
-  -h, --help            show this help message and
-                        exit
-  -v, --version         show program's version number
-                        and exit
+  -h, --help            show this help message and exit
+  -v, --version         show program's version number and exit
   -f mp4|mp3, --format mp4|mp3
-                        Specify media type -
-                        audio/video
+                        Specify media type - audio/video
   -q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps, --quality 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps
                         Media quality -720p
   -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3
-                        Other media formats incase of
-                        multiple options - mp4/mp3
+                        Other media formats incase of multiple
+                        options - mp4/mp3
   -k [KEYWORD ...], --keyword [KEYWORD ...]
-                        Media should contain this
-                        keywords - None
+                        Media should contain this keywords -
+                        None
   -a [AUTHOR ...], --author [AUTHOR ...]
-                        Media author i.e YouTube
-                        channel name - None
+                        Media author i.e YouTube channel name -
+                        None
   -l LIMIT, --limit LIMIT
-                        Total videos to be downloaded
-                        - 1
-  -d PATH, --dir PATH   Directory for saving the
-                        contents - /storage/emulated/
-                        0/git/Smartwa/y2mate-api
+                        Total videos to be downloaded - 1
+  -d PATH, --dir PATH   Directory for saving the contents -
+                        /storage/emulated/0/git/Smartwa
   -t TIMEOUT, --timeout TIMEOUT
                         Http request timeout - 30s
   -i PATH, --input PATH
-                        Path to text file containing
-                        query per line - None
-  --disable-bar         Disables download progress
-                        bar - False
-  --ask                 Confirm before downloading
-                        file - False
-  --unique              Auto-skip any media that you
-                        once dowloaded - False
-  --history             Stdout all media metadata
-                        ever downloaded - False
-  --clear               Clear all download histories
-                        - False
+                        Path to text file containing query per
+                        line - None
+  -thr THREAD, --thread THREAD
+                        Download [x] amount of videos/audios at
+                        once - 1
+  --disable-bar         Disables download progress bar - False
+  --ask                 Confirm before downloading file - False
+  --unique              Auto-skip any media that you once
+                        dowloaded - False
+  --quiet               Not to stdout anything other than logs -
+                        False
+  --history             Stdout all media metadata ever
+                        downloaded - False
+  --clear               Clear all download histories - False
 
 This script has no official relation with y2mate.com
 ```
 </details>
 
 - Review [CHANGELOG](https://github.com/Simatwa/y2mate-api/blob/main/Docs/CHANGELOG.md) for latest updates.
```

#### html2text {}

```diff
@@ -52,34 +52,37 @@
 `Handler.run` * progress_bar : Stdout media-name & Display progress bar -
 `Handler.save` * third_dict : Response of `third_query.run()` * dir : Directory
 for saving the contents * progress_bar : Stdout media-name & Display download
 progress bar    For more info run `$ y2mate -h`  ``` usage: y2mate [-h] [-v] [-
 f mp4|mp3] [-
 q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
 [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]] [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
-[-t TIMEOUT] [-i PATH] [--disable-bar] [--ask] [--unique] [--history] [--clear]
-[query ...] Download youtube videos and audios by title or link positional
-arguments: query Youtube video title, link or id - None options: -h, --help
-show this help message and exit -v, --version show program's version number and
-exit -f mp4|mp3, --format mp4|mp3 Specify media type - audio/video -
+[-t TIMEOUT] [-i PATH] [-thr THREAD] [--disable-bar] [--ask] [--unique] [--
+quiet] [--history] [--clear] [query ...] Download youtube videos and audios by
+title or link positional arguments: query Youtube video title, link or id -
+None options: -h, --help show this help message and exit -v, --version show
+program's version number and exit -f mp4|mp3, --format mp4|mp3 Specify media
+type - audio/video -
 q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps,
 --quality
 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps
 Media quality -720p -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3 Other media
 formats incase of multiple options - mp4/mp3 -k [KEYWORD ...], --keyword
 [KEYWORD ...] Media should contain this keywords - None -a [AUTHOR ...], --
 author [AUTHOR ...] Media author i.e YouTube channel name - None -l LIMIT, --
 limit LIMIT Total videos to be downloaded - 1 -d PATH, --dir PATH Directory for
-saving the contents - /storage/emulated/ 0/git/Smartwa/y2mate-api -t TIMEOUT, -
--timeout TIMEOUT Http request timeout - 30s -i PATH, --input PATH Path to text
-file containing query per line - None --disable-bar Disables download progress
+saving the contents - /storage/emulated/0/git/Smartwa -t TIMEOUT, --timeout
+TIMEOUT Http request timeout - 30s -i PATH, --input PATH Path to text file
+containing query per line - None -thr THREAD, --thread THREAD Download [x]
+amount of videos/audios at once - 1 --disable-bar Disables download progress
 bar - False --ask Confirm before downloading file - False --unique Auto-skip
-any media that you once dowloaded - False --history Stdout all media metadata
-ever downloaded - False --clear Clear all download histories - False This
-script has no official relation with y2mate.com ```  - Review [CHANGELOG]
-(https://github.com/Simatwa/y2mate-api/blob/main/Docs/CHANGELOG.md) for latest
-updates. ## Disclaimer This repository is intended for educational and personal
-use only. The use of this repository for any commercial or illegal purposes is
-strictly prohibited. The repository owner does not endorse or encourage the
-downloading or sharing of copyrighted material without permission. The
-repository owner is not responsible for any misuse of the software or any legal
-consequences that may arise from such misuse.
+any media that you once dowloaded - False --quiet Not to stdout anything other
+than logs - False --history Stdout all media metadata ever downloaded - False -
+-clear Clear all download histories - False This script has no official
+relation with y2mate.com ```  - Review [CHANGELOG](https://github.com/Simatwa/
+y2mate-api/blob/main/Docs/CHANGELOG.md) for latest updates. ## Disclaimer This
+repository is intended for educational and personal use only. The use of this
+repository for any commercial or illegal purposes is strictly prohibited. The
+repository owner does not endorse or encourage the downloading or sharing of
+copyrighted material without permission. The repository owner is not
+responsible for any misuse of the software or any legal consequences that may
+arise from such misuse.
```

### Comparing `y2mate-api-0.0.2/setup.py` & `y2mate-api-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     project_urls={"Bug Report": f"{__repo__}/issues/new"},
     install_requires=[
         "argparse>=1.1",
         "requests>=2.0.2",
         "tqdm==4.65.0",
         "colorama==0.4.6",
         "appdirs==1.4.4",
+        "getch==1.0",
     ],
     python_requires=">=3.8",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Development Status :: 4 - Beta",
```

### Comparing `y2mate-api-0.0.2/y2mate_api/console.py` & `y2mate-api-0.0.3/y2mate_api/console.py`

 * *Files 9% similar despite different names*

```diff
@@ -94,14 +94,21 @@
     parser.add_argument(
         "-i",
         "--input",
         help="Path to text file containing query per line - %(default)s",
         metavar="PATH",
     )
     parser.add_argument(
+        "-thr",
+        "--thread",
+        help="Download [x] amount of videos/audios at once - 1",
+        type=int,
+        default=0,
+    )
+    parser.add_argument(
         "--disable-bar",
         help="Disables download progress bar - %(default)s",
         action="store_true",
     )
     parser.add_argument(
         "--ask",
         help="Confirm before downloading file - %(default)s",
@@ -109,14 +116,19 @@
     )
     parser.add_argument(
         "--unique",
         help="Auto-skip any media that you once dowloaded - %(default)s",
         action="store_true",
     )
     parser.add_argument(
+        "--quiet",
+        help="Not to stdout anything other than logs - %(default)s",
+        action="store_true",
+    )
+    parser.add_argument(
         "--history",
         help="Stdout all media metadata ever downloaded - %(default)s",
         action="store_true",
     )
     parser.add_argument(
         "--clear",
         help="Clear all download histories - %(default)s",
@@ -142,18 +154,20 @@
     h_mult_args = lambda v: v if not v else " ".join(v)
     handler_init_args = dict(
         query=h_mult_args(args.query),
         author=args.author,
         timeout=args.timeout,
         ask=args.ask,
         unique=args.unique,
+        thread=args.thread,
     )
     auto_save_args = dict(
         dir=args.dir,
         progress_bar=args.disable_bar == False,
+        quiet=args.quiet,
         format=args.format,
         quality=args.quality,
         resolver=args.resolver,
         limit=args.limit,
         keyword=h_mult_args(args.keyword),
         author=h_mult_args(args.author),
     )
@@ -161,8 +175,10 @@
     if args.input:
         for query in open(args.input).read().strip().split("\n"):
             handler_init_args["query"] = query
             auto_save_args["limit"] = 1
             Handler(**handler_init_args).auto_save(**auto_save_args)
     else:
         Handler(**handler_init_args).auto_save(**auto_save_args)
-    logging.info("Done downloading mp3/mp4")
+    logging.info(
+        f"Done downloading [{args.limit}] {'audio' if args.format=='mp3' else 'video'}(s)"
+    )
```

### Comparing `y2mate-api-0.0.2/y2mate_api/downloader.py` & `y2mate-api-0.0.3/y2mate_api/downloader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from .main import requests, logging, utils, first_query, second_query, third_query
 from tqdm import tqdm
 from colorama import Fore
-from os import path
+from os import path, getcwd
+from threading import Thread
+from getch import getch
+from sys import stdout
 
 """
 - query string
 - format mp4/3
 - quality 720p/128kbps
 - keywords
 - Specify video author
@@ -21,33 +24,37 @@
     def __init__(
         self,
         query: str,
         author: str = None,
         timeout: int = 30,
         ask: bool = False,
         unique: bool = False,
+        thread: int = 0,
     ):
         r"""Initializes this `class`
         :param query: Video name or youtube link
         :type query: str
         :param author: (Optional) Author (Channel) of the videos
         :type author: str
         :param timeout: (Optional) Http request timeout
         :type timeout: int
         :param ask: (Optional) Confirm before downloading media
         :type ask: bool
         :param unique: (Optional) Ignore previously downloaded media
         :type ask: bool
+        :param thread: (Optional) Thread the download process through `auto-save` method
+        :type thread int
         """
         self.query = query
         self.author = author
         self.timeout = timeout
         self.keyword = None
         self.ask = ask
         self.unique = unique
+        self.thread = thread
         self.vitems = []
         self.related = []
         self.total = 1
         self.saved_videos = utils.get_history()
 
     def __str__(self):
         return self.query
@@ -82,55 +89,66 @@
     def __make_first_query(self):
         r"""Sets query_one attribute to `self`"""
         query_one = first_query(self.query)
         self.__setattr__("query_one", query_one.main(self.timeout))
         if self.query_one.is_link == False:
             self.vitems.extend(self.__filter_videos(self.query_one.vitems))
 
+    @utils.error_handler(exit_on_error=True)
     def __verify_item(self, second_query_obj) -> bool:
         video_id = second_query_obj.vid
         video_author = second_query_obj.a
         video_title = second_query_obj.title
         confirm = lambda choice: True if choice.lower() in ("yes", "y") else False
         if video_id in self.saved_videos:
             if self.unique:
                 return False, "Duplicate"
             if self.ask:
-                choice = input(
-                    f">> Re-download : {Fore.GREEN+video_title+Fore.RESET} by {Fore.YELLOW+video_author+Fore.RESET}? - [y/N] :"
+                stdout.write(
+                    f">> Re-download : {Fore.GREEN+video_title+Fore.RESET} by {Fore.YELLOW+video_author+Fore.RESET} - [y/N]? :"
                 )
+                stdout.flush()
+                choice = getch()
+                print("\n[*] Ok processing...", end="\r")
                 return confirm(choice), "User's choice"
         if self.ask:
-            choice = input(
-                f">> Download : {Fore.GREEN+video_title+Fore.RESET} by {Fore.YELLOW+video_author+Fore.RESET}? - [Y/n] :"
+            stdout.write(
+                f">> Download : {Fore.GREEN+video_title+Fore.RESET} by {Fore.YELLOW+video_author+Fore.RESET} - [Y/n]? :"
             )
+            stdout.flush()
+            choice = getch()
+            print("\n[*] Ok processing...", end="\r")
             return confirm(choice), "User's choice"
         return True, "Auto"
 
     def __make_second_query(self):
         r"""Links first query with 3rd query"""
         init_query_two = second_query(self.query_one)
+        x = 0
         if not self.query_one.is_link:
-            for x, video_dict in enumerate(self.vitems):
+            for video_dict in self.vitems:
                 init_query_two.video_dict = video_dict
                 query_2 = init_query_two.main(timeout=self.timeout)
                 if query_2.processed:
                     if self.author and not self.author.lower() in query_2.a.lower():
-                        logging.warning(f"Dropping '{query_2.title}' by  '{query_2.a}'")
+                        logging.warning(
+                            f"Dropping {Fore.YELLOW+query_2.title+Fore.RESET} by  {Fore.RED+query_2.a+Fore.RESET}"
+                        )
                         continue
                     else:
                         yes_download, reason = self.__verify_item(query_2)
                         if not yes_download:
                             logging.warning(
-                                f"Skipping '{query_2.title}' by '{query_2.a}' -  Reason : {reason}"
+                                f"Skipping {Fore.YELLOW+query_2.title+Fore.RESET} by {Fore.MAGENTA+query_2.a+Fore.RESET} -  Reason : {Fore.BLUE+reason+Fore.RESET}"
                             )
                             continue
                         self.related.append(query_2.related)
                         yield query_2
-                        if x + 1 >= self.total:
+                        x += 1
+                        if x >= self.total:
                             break
                 else:
                     logging.warning(
                         f"Dropping unprocessed query_two object of index {x}"
                     )
 
         else:
@@ -138,37 +156,38 @@
             if query_2.processed:
                 # self.related.extend(query_2.related)
                 self.vitems.extend(query_2.related)
                 self.query_one.is_link = False
                 if self.total == 1:
                     yield query_2
                 else:
-                    for x, video_dict in enumerate(self.vitems):
+                    for video_dict in self.vitems:
                         init_query_two.video_dict = video_dict
                         query_2 = init_query_two.main(timeout=self.timeout)
                         if query_2.processed:
                             if (
                                 self.author
                                 and not self.author.lower() in query_2.a.lower()
                             ):
                                 logging.warning(
-                                    f"Dropping '{query_2.title}' by  '{query_2.a}'"
+                                    f"Dropping {Fore.YELLOW+query_2.title+Fore.RESET} by  {Fore.RED+query_2.a+Fore.RESET}"
                                 )
                                 continue
                             else:
                                 yes_download, reason = self.__verify_item(query_2)
                                 if not yes_download:
                                     logging.warning(
-                                        f"Skipping `{query_2.title}` by `{query_2.a}` -  Reason : {reason}"
+                                        f"Skipping {Fore.YELLOW+query_2.title+Fore.RESET} by {Fore.MAGENTA+query_2.a+Fore.RESET} -  Reason : {Fore.BLUE+reason+Fore.RESET}"
                                     )
                                     continue
 
                                 self.related.append(query_2.related)
                                 yield query_2
-                                if x + 1 >= self.total:
+                                x += 1
+                                if x >= self.total:
                                     break
                         else:
                             logging.warning(
                                 f"Dropping unprocessed query_two object of index {x}"
                             )
                             yield
             else:
@@ -214,15 +233,15 @@
                 )
             else:
                 logging.error(f"Empty object - {query_two_obj}")
 
     def generate_filename(self, third_dict: dict, format: str = None) -> str:
         r"""Generate filename based on the response of `third_query`
         :param third_dict: response of `third_query.main()` object
-        :param format: Format for formatting fnm based on `third_dict` keys
+        :param format: (Optional) Format for formatting fnm based on `third_dict` keys
         :type third_dict: dict
         :type format: str
         :rtype: str
         """
         fnm = (
             f"{format}" % third_dict
             if format
@@ -234,62 +253,98 @@
             for val in trash:
                 nm = nm.replace(val, "")
             return nm
 
         return sanitize(fnm)
 
     def auto_save(
-        self, dir: str = "", iterator: object = None, progress_bar=True, *args, **kwargs
+        self,
+        dir: str = "",
+        iterator: object = None,
+        progress_bar=True,
+        quiet: bool = False,
+        *args,
+        **kwargs,
     ):
         r"""Query and save all the media
-        :param dir: Path to Directory for saving the media files
-        :param iterator: Function that yields third_query object - `Handler.run`
-        :param progress_bar: Display progress bar
+        :param dir: (Optional) Path to Directory for saving the media files
+        :param iterator: (Optional) Function that yields third_query object - `Handler.run`
+        :param progress_bar: (Optional) Display progress bar
+        :param quiet: (Optional) Not to stdout anything
         :type dir: str
         :type iterator: object
         :type progress_bar: bool
+        :type quiet: bool
         args & kwargs for the iterator
         :rtype: None
         """
         iterator_object = iterator or self.run(*args, **kwargs)
 
-        for entry in iterator_object:
+        for x, entry in enumerate(iterator_object):
 
-            self.save(entry, dir, progress_bar)
+            if self.thread:
+                t1 = Thread(
+                    target=self.save,
+                    args=(
+                        entry,
+                        dir,
+                        False,
+                        quiet,
+                    ),
+                )
+                t1.start()
+                thread_count = x + 1
+                if thread_count % self.thread == 0 or thread_count == self.total:
+                    logging.debug(
+                        f"Waiting for current running threads to finish - thread_count : {thread_count}"
+                    )
+                    t1.join()
+            else:
+                self.save(entry, dir, progress_bar, quiet)
 
-    def save(self, third_dict: dict, dir: str = "", progress_bar=True):
+    def save(
+        self, third_dict: dict, dir: str = "", progress_bar=True, quiet: bool = False
+    ):
         r"""Download media based on response of `third_query` dict-data-type
         :param third_dict: Response of `third_query.run()`
-        :param dir: Directory for saving the contents
-        :param progress_bar: Display download progress bar
+        :param dir: (Optional) Directory for saving the contents
+        :param progress_bar: (Optional) Display download progress bar
+        :param quiet: (Optional) Not to stdout anything
         :type third_dict: dict
         :type dir: str
         :type progress_bar: bool
+        :type quiet: bool
         :rtype: None
         """
         if third_dict:
             resp = requests.get(third_dict["dlink"], stream=True)
             size_in_bits = int(resp.headers["content-length"])
             size_in_mb = round(size_in_bits / 1000000, 2)
             chunk_size = 1024
             filename = self.generate_filename(third_dict)
-
+            save_to = path.join(dir, filename)
+            third_dict["saved_to"] = (
+                save_to
+                if save_to.startswith(("/", "C:", "D:"))
+                else path.join(getcwd(), dir, filename)
+            )
             if progress_bar:
-                print(f"{filename}")
+                if not quiet:
+                    print(f"{filename}")
                 with tqdm(
                     total=size_in_bits,
                     bar_format="%s%d MB %s{bar} %s{l_bar}%s"
                     % (Fore.GREEN, size_in_mb, Fore.CYAN, Fore.YELLOW, Fore.RESET),
                 ) as p_bar:
-                    with open(path.join(dir, filename), "wb") as fh:
+                    with open(save_to, "wb") as fh:
                         for chunks in resp.iter_content(chunk_size=chunk_size):
                             fh.write(chunks)
                             p_bar.update(chunk_size)
                     utils.add_history(third_dict)
             else:
-                with open(path.join(dir, filename), "wb") as fh:
+                with open(save_to, "wb") as fh:
                     for chunks in resp.iter_content(chunk_size=chunk_size):
                         fh.write(chunks)
                 utils.add_history(third_dict)
                 logging.info(f"{filename} - {size_in_mb}MB ✅")
         else:
             logging.error(f"Empty `third_dict` parameter parsed : {third_dict}")
```

### Comparing `y2mate-api-0.0.2/y2mate_api/main.py` & `y2mate-api-0.0.3/y2mate_api/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import requests
 import logging
 from time import sleep
 import json
 from os import path, makedirs
 from datetime import datetime
 from appdirs import AppDirs
+from sys import exit
 
 __prog__ = "y2mate"
 session = requests.session()
 
 headers = {
     "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
     "User-Agent": "Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Mobile Safari/537.36",
@@ -38,20 +39,22 @@
     @staticmethod
     def error_handler(resp=None, exit_on_error=False, log=True):
         r"""Execption handler decorator"""
 
         def decorator(func):
             def main(*args, **kwargs):
                 try:
-                    return func(*args, **kwargs)
+                    try:
+                        return func(*args, **kwargs)
+                    except (KeyboardInterrupt) as e:
+                        logging.info(f"^KeyboardInterrupt quitting. Goodbye!")
+                        exit(1)
                 except Exception as e:
-                    # import traceback as tb
-
-                    # tb.print_exc()
                     if log:
+                        # logging.exception(e)
                         logging.debug(f"Function ({func.__name__}) : {get_excep(e)}")
                         logging.error(get_excep(e))
                     if exit_on_error:
                         exit(1)
 
                     return resp
```

### Comparing `y2mate-api-0.0.2/y2mate_api.egg-info/PKG-INFO` & `y2mate-api-0.0.3/y2mate_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y2mate-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: Download youtube videos and audios by title or link
 Home-page: https://github.com/Simatwa/y2mate-api
 Author: Smartwa
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/y2mate-api/issues/new
@@ -27,15 +27,15 @@
 License-File: LICENSE
 
 # y2mate-api
 
 <p align="center">
 <a href="https://github.com/Simatwa/y2mate-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.2&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.3&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
 
@@ -188,65 +188,61 @@
 </summary>
 
 ```
 usage: y2mate [-h] [-v] [-f mp4|mp3]
               [-q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
               [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]]
               [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
-              [-t TIMEOUT] [-i PATH] [--disable-bar]
-              [--ask] [--unique] [--history]
-              [--clear]
+              [-t TIMEOUT] [-i PATH] [-thr THREAD]
+              [--disable-bar] [--ask] [--unique] [--quiet]
+              [--history] [--clear]
               [query ...]
 
 Download youtube videos and audios by title or link
 
 positional arguments:
-  query                 Youtube video title, link or
-                        id - None
+  query                 Youtube video title, link or id - None
 
 options:
-  -h, --help            show this help message and
-                        exit
-  -v, --version         show program's version number
-                        and exit
+  -h, --help            show this help message and exit
+  -v, --version         show program's version number and exit
   -f mp4|mp3, --format mp4|mp3
-                        Specify media type -
-                        audio/video
+                        Specify media type - audio/video
   -q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps, --quality 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps
                         Media quality -720p
   -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3
-                        Other media formats incase of
-                        multiple options - mp4/mp3
+                        Other media formats incase of multiple
+                        options - mp4/mp3
   -k [KEYWORD ...], --keyword [KEYWORD ...]
-                        Media should contain this
-                        keywords - None
+                        Media should contain this keywords -
+                        None
   -a [AUTHOR ...], --author [AUTHOR ...]
-                        Media author i.e YouTube
-                        channel name - None
+                        Media author i.e YouTube channel name -
+                        None
   -l LIMIT, --limit LIMIT
-                        Total videos to be downloaded
-                        - 1
-  -d PATH, --dir PATH   Directory for saving the
-                        contents - /storage/emulated/
-                        0/git/Smartwa/y2mate-api
+                        Total videos to be downloaded - 1
+  -d PATH, --dir PATH   Directory for saving the contents -
+                        /storage/emulated/0/git/Smartwa
   -t TIMEOUT, --timeout TIMEOUT
                         Http request timeout - 30s
   -i PATH, --input PATH
-                        Path to text file containing
-                        query per line - None
-  --disable-bar         Disables download progress
-                        bar - False
-  --ask                 Confirm before downloading
-                        file - False
-  --unique              Auto-skip any media that you
-                        once dowloaded - False
-  --history             Stdout all media metadata
-                        ever downloaded - False
-  --clear               Clear all download histories
-                        - False
+                        Path to text file containing query per
+                        line - None
+  -thr THREAD, --thread THREAD
+                        Download [x] amount of videos/audios at
+                        once - 1
+  --disable-bar         Disables download progress bar - False
+  --ask                 Confirm before downloading file - False
+  --unique              Auto-skip any media that you once
+                        dowloaded - False
+  --quiet               Not to stdout anything other than logs -
+                        False
+  --history             Stdout all media metadata ever
+                        downloaded - False
+  --clear               Clear all download histories - False
 
 This script has no official relation with y2mate.com
 ```
 </details>
 
 - Review [CHANGELOG](https://github.com/Simatwa/y2mate-api/blob/main/Docs/CHANGELOG.md) for latest updates.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.2 Summary: Download youtube
+Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.3 Summary: Download youtube
 videos and audios by title or link Home-page: https://github.com/Simatwa/
 y2mate-api Author: Smartwa Author-email: smartwacaleb@gmail.com Maintainer:
 Smartwa License: MIT Project-URL: Bug Report, https://github.com/Simatwa/
 y2mate-api/issues/new Keywords: y2mate,videos,video-api,youtube Classifier:
 License :: OSI Approved :: MIT License Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: Free For Home Use Classifier: Intended
@@ -66,34 +66,37 @@
 `Handler.run` * progress_bar : Stdout media-name & Display progress bar -
 `Handler.save` * third_dict : Response of `third_query.run()` * dir : Directory
 for saving the contents * progress_bar : Stdout media-name & Display download
 progress bar    For more info run `$ y2mate -h`  ``` usage: y2mate [-h] [-v] [-
 f mp4|mp3] [-
 q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
 [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]] [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
-[-t TIMEOUT] [-i PATH] [--disable-bar] [--ask] [--unique] [--history] [--clear]
-[query ...] Download youtube videos and audios by title or link positional
-arguments: query Youtube video title, link or id - None options: -h, --help
-show this help message and exit -v, --version show program's version number and
-exit -f mp4|mp3, --format mp4|mp3 Specify media type - audio/video -
+[-t TIMEOUT] [-i PATH] [-thr THREAD] [--disable-bar] [--ask] [--unique] [--
+quiet] [--history] [--clear] [query ...] Download youtube videos and audios by
+title or link positional arguments: query Youtube video title, link or id -
+None options: -h, --help show this help message and exit -v, --version show
+program's version number and exit -f mp4|mp3, --format mp4|mp3 Specify media
+type - audio/video -
 q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps,
 --quality
 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps
 Media quality -720p -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3 Other media
 formats incase of multiple options - mp4/mp3 -k [KEYWORD ...], --keyword
 [KEYWORD ...] Media should contain this keywords - None -a [AUTHOR ...], --
 author [AUTHOR ...] Media author i.e YouTube channel name - None -l LIMIT, --
 limit LIMIT Total videos to be downloaded - 1 -d PATH, --dir PATH Directory for
-saving the contents - /storage/emulated/ 0/git/Smartwa/y2mate-api -t TIMEOUT, -
--timeout TIMEOUT Http request timeout - 30s -i PATH, --input PATH Path to text
-file containing query per line - None --disable-bar Disables download progress
+saving the contents - /storage/emulated/0/git/Smartwa -t TIMEOUT, --timeout
+TIMEOUT Http request timeout - 30s -i PATH, --input PATH Path to text file
+containing query per line - None -thr THREAD, --thread THREAD Download [x]
+amount of videos/audios at once - 1 --disable-bar Disables download progress
 bar - False --ask Confirm before downloading file - False --unique Auto-skip
-any media that you once dowloaded - False --history Stdout all media metadata
-ever downloaded - False --clear Clear all download histories - False This
-script has no official relation with y2mate.com ```  - Review [CHANGELOG]
-(https://github.com/Simatwa/y2mate-api/blob/main/Docs/CHANGELOG.md) for latest
-updates. ## Disclaimer This repository is intended for educational and personal
-use only. The use of this repository for any commercial or illegal purposes is
-strictly prohibited. The repository owner does not endorse or encourage the
-downloading or sharing of copyrighted material without permission. The
-repository owner is not responsible for any misuse of the software or any legal
-consequences that may arise from such misuse.
+any media that you once dowloaded - False --quiet Not to stdout anything other
+than logs - False --history Stdout all media metadata ever downloaded - False -
+-clear Clear all download histories - False This script has no official
+relation with y2mate.com ```  - Review [CHANGELOG](https://github.com/Simatwa/
+y2mate-api/blob/main/Docs/CHANGELOG.md) for latest updates. ## Disclaimer This
+repository is intended for educational and personal use only. The use of this
+repository for any commercial or illegal purposes is strictly prohibited. The
+repository owner does not endorse or encourage the downloading or sharing of
+copyrighted material without permission. The repository owner is not
+responsible for any misuse of the software or any legal consequences that may
+arise from such misuse.
```

