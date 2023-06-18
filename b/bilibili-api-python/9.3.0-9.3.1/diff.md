# Comparing `tmp/bilibili-api-python-9.3.0.tar.gz` & `tmp/bilibili-api-python-9.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bilibili-api-python-9.3.0.tar", last modified: Sun May  8 12:02:27 2022, max compression
+gzip compressed data, was "bilibili-api-python-9.3.1.tar", last modified: Mon May  9 03:14:54 2022, max compression
```

## Comparing `bilibili-api-python-9.3.0.tar` & `bilibili-api-python-9.3.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxrwx   0        0        0        0 2022-05-08 12:02:27.567704 bilibili-api-python-9.3.0/
--rw-rw-rw-   0        0        0    35821 2022-04-27 12:51:37.000000 bilibili-api-python-9.3.0/LICENSE
--rw-rw-rw-   0        0        0     6766 2022-05-08 12:02:27.564742 bilibili-api-python-9.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     6033 2022-04-27 12:51:37.000000 bilibili-api-python-9.3.0/README.md
-drwxrwxrwx   0        0        0        0 2022-05-08 12:02:27.229383 bilibili-api-python-9.3.0/bilibili_api/
--rw-rw-rw-   0        0        0      462 2022-04-29 05:16:25.000000 bilibili-api-python-9.3.0/bilibili_api/__init__.py
--rw-rw-rw-   0        0        0     2835 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/app.py
--rw-rw-rw-   0        0        0    23548 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/article.py
--rw-rw-rw-   0        0        0     3767 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/audio.py
--rw-rw-rw-   0        0        0     6735 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/bangumi.py
--rw-rw-rw-   0        0        0     2603 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/channel.py
--rw-rw-rw-   0        0        0     7778 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/comment.py
-drwxrwxrwx   0        0        0        0 2022-05-08 12:02:27.236364 bilibili-api-python-9.3.0/bilibili_api/data/
-drwxrwxrwx   0        0        0        0 2022-05-08 12:02:27.331533 bilibili-api-python-9.3.0/bilibili_api/data/api/
--rw-rw-rw-   0        0        0      244 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/data/api/README.md
--rw-rw-rw-   0        0        0      861 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/data/api/app.json
--rw-rw-rw-   0        0        0     1621 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/data/api/article.json
--rw-rw-rw-   0        0        0     2938 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/data/api/audio.json
--rw-rw-rw-   0        0        0     3312 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/data/api/bangumi.json
--rw-rw-rw-   0        0        0      319 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/data/api/channel.json
--rw-rw-rw-   0        0        0     6153 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/data/api/common.json
--rw-rw-rw-   0        0        0     5695 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/data/api/dynamic.json
--rw-rw-rw-   0        0        0     5479 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/data/api/favorite-list.json
--rw-rw-rw-   0        0        0      904 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/data/api/interactive_video.json
--rw-rw-rw-   0        0        0    14447 2022-04-27 12:09:52.000000 bilibili-api-python-9.3.0/bilibili_api/data/api/live.json
--rw-rw-rw-   0        0        0      809 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/data/api/misc.json
--rw-rw-rw-   0        0        0     9061 2022-05-08 11:53:45.000000 bilibili-api-python-9.3.0/bilibili_api/data/api/user.json
--rw-rw-rw-   0        0        0     9530 2022-05-03 01:46:08.000000 bilibili-api-python-9.3.0/bilibili_api/data/api/video.json
--rw-rw-rw-   0        0        0     2647 2022-04-27 12:09:52.000000 bilibili-api-python-9.3.0/bilibili_api/data/api/video_uploader.json
--rw-rw-rw-   0        0        0    42778 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/data/channel.json
--rw-rw-rw-   0        0        0    11083 2022-05-07 02:59:50.000000 bilibili-api-python-9.3.0/bilibili_api/dynamic.py
-drwxrwxrwx   0        0        0        0 2022-05-08 12:02:27.411539 bilibili-api-python-9.3.0/bilibili_api/exceptions/
--rw-rw-rw-   0        0        0      344 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/exceptions/ApiException.py
--rw-rw-rw-   0        0        0      362 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/exceptions/ArgsException.py
--rw-rw-rw-   0        0        0      396 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/exceptions/CredentialNoBiliJctException.py
--rw-rw-rw-   0        0        0      390 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/exceptions/CredentialNoBuvid3Exception.py
--rw-rw-rw-   0        0        0      398 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/exceptions/CredentialNoSessdataException.py
--rw-rw-rw-   0        0        0      337 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/exceptions/DanmakuClosedException.py
--rw-rw-rw-   0        0        0      355 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/exceptions/DynamicExceedImagesException.py
--rw-rw-rw-   0        0        0      220 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/exceptions/LiveException.py
--rw-rw-rw-   0        0        0      555 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/exceptions/NetworkException.py
--rw-rw-rw-   0        0        0      727 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/exceptions/ResponseCodeException.py
--rw-rw-rw-   0        0        0      378 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/exceptions/ResponseException.py
--rw-rw-rw-   0        0        0      388 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/exceptions/VideoUploadException.py
--rw-rw-rw-   0        0        0      331 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/exceptions/__init__.py
--rw-rw-rw-   0        0        0    11478 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/favorite_list.py
--rw-rw-rw-   0        0        0     3415 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/interactive_video.py
--rw-rw-rw-   0        0        0    37485 2022-04-27 12:09:52.000000 bilibili-api-python-9.3.0/bilibili_api/live.py
--rw-rw-rw-   0        0        0     1043 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/misc.py
--rw-rw-rw-   0        0        0      102 2022-05-05 03:22:03.000000 bilibili-api-python-9.3.0/bilibili_api/settings.py
--rw-rw-rw-   0        0        0    19345 2022-05-08 11:53:45.000000 bilibili-api-python-9.3.0/bilibili_api/user.py
-drwxrwxrwx   0        0        0        0 2022-05-08 12:02:27.467655 bilibili-api-python-9.3.0/bilibili_api/utils/
--rw-rw-rw-   0        0        0     2164 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/utils/AsyncEvent.py
--rw-rw-rw-   0        0        0     5134 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/utils/BytesReader.py
--rw-rw-rw-   0        0        0     2292 2022-04-27 12:09:52.000000 bilibili-api-python-9.3.0/bilibili_api/utils/Credential.py
--rw-rw-rw-   0        0        0     3214 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/utils/Danmaku.py
--rw-rw-rw-   0        0        0        0 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/utils/__init__.py
--rw-rw-rw-   0        0        0     1258 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/utils/aid_bvid_transformer.py
--rw-rw-rw-   0        0        0     5557 2022-05-07 10:39:14.000000 bilibili-api-python-9.3.0/bilibili_api/utils/network.py
--rw-rw-rw-   0        0        0      586 2022-04-27 12:09:52.000000 bilibili-api-python-9.3.0/bilibili_api/utils/sync.py
--rw-rw-rw-   0        0        0     4173 2022-04-27 12:09:52.000000 bilibili-api-python-9.3.0/bilibili_api/utils/utils.py
--rw-rw-rw-   0        0        0      598 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.0/bilibili_api/utils/varint.py
--rw-rw-rw-   0        0        0    45752 2022-05-07 03:03:56.000000 bilibili-api-python-9.3.0/bilibili_api/video.py
--rw-rw-rw-   0        0        0    24110 2022-04-27 12:09:52.000000 bilibili-api-python-9.3.0/bilibili_api/video_uploader.py
-drwxrwxrwx   0        0        0        0 2022-05-08 12:02:27.554655 bilibili-api-python-9.3.0/bilibili_api_python.egg-info/
--rw-rw-rw-   0        0        0     6766 2022-05-08 12:02:26.000000 bilibili-api-python-9.3.0/bilibili_api_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2126 2022-05-08 12:02:26.000000 bilibili-api-python-9.3.0/bilibili_api_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-08 12:02:26.000000 bilibili-api-python-9.3.0/bilibili_api_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2022-05-08 12:02:26.000000 bilibili-api-python-9.3.0/bilibili_api_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-05-08 12:02:26.000000 bilibili-api-python-9.3.0/bilibili_api_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-08 12:02:27.568685 bilibili-api-python-9.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1282 2022-05-08 12:00:40.000000 bilibili-api-python-9.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-05-09 03:14:54.293326 bilibili-api-python-9.3.1/
+-rw-rw-rw-   0        0        0    35821 2022-04-27 12:51:37.000000 bilibili-api-python-9.3.1/LICENSE
+-rw-rw-rw-   0        0        0     6766 2022-05-09 03:14:54.291330 bilibili-api-python-9.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6033 2022-04-27 12:51:37.000000 bilibili-api-python-9.3.1/README.md
+drwxrwxrwx   0        0        0        0 2022-05-09 03:14:54.150325 bilibili-api-python-9.3.1/bilibili_api/
+-rw-rw-rw-   0        0        0      462 2022-04-29 05:16:25.000000 bilibili-api-python-9.3.1/bilibili_api/__init__.py
+-rw-rw-rw-   0        0        0     2835 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/app.py
+-rw-rw-rw-   0        0        0    23548 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/article.py
+-rw-rw-rw-   0        0        0     3767 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/audio.py
+-rw-rw-rw-   0        0        0     6735 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/bangumi.py
+-rw-rw-rw-   0        0        0     2603 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/channel.py
+-rw-rw-rw-   0        0        0     7778 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/comment.py
+drwxrwxrwx   0        0        0        0 2022-05-09 03:14:54.153326 bilibili-api-python-9.3.1/bilibili_api/data/
+drwxrwxrwx   0        0        0        0 2022-05-09 03:14:54.198325 bilibili-api-python-9.3.1/bilibili_api/data/api/
+-rw-rw-rw-   0        0        0      244 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/data/api/README.md
+-rw-rw-rw-   0        0        0      861 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/data/api/app.json
+-rw-rw-rw-   0        0        0     1621 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/data/api/article.json
+-rw-rw-rw-   0        0        0     2938 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/data/api/audio.json
+-rw-rw-rw-   0        0        0     3312 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/data/api/bangumi.json
+-rw-rw-rw-   0        0        0      319 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/data/api/channel.json
+-rw-rw-rw-   0        0        0     6153 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/data/api/common.json
+-rw-rw-rw-   0        0        0     5695 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/data/api/dynamic.json
+-rw-rw-rw-   0        0        0     5479 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/data/api/favorite-list.json
+-rw-rw-rw-   0        0        0      904 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/data/api/interactive_video.json
+-rw-rw-rw-   0        0        0    14447 2022-04-27 12:09:52.000000 bilibili-api-python-9.3.1/bilibili_api/data/api/live.json
+-rw-rw-rw-   0        0        0      809 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/data/api/misc.json
+-rw-rw-rw-   0        0        0     9186 2022-05-09 02:22:39.000000 bilibili-api-python-9.3.1/bilibili_api/data/api/user.json
+-rw-rw-rw-   0        0        0     9530 2022-05-03 01:46:08.000000 bilibili-api-python-9.3.1/bilibili_api/data/api/video.json
+-rw-rw-rw-   0        0        0     2647 2022-04-27 12:09:52.000000 bilibili-api-python-9.3.1/bilibili_api/data/api/video_uploader.json
+-rw-rw-rw-   0        0        0    42778 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/data/channel.json
+-rw-rw-rw-   0        0        0    11083 2022-05-07 02:59:50.000000 bilibili-api-python-9.3.1/bilibili_api/dynamic.py
+drwxrwxrwx   0        0        0        0 2022-05-09 03:14:54.237322 bilibili-api-python-9.3.1/bilibili_api/exceptions/
+-rw-rw-rw-   0        0        0      344 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/exceptions/ApiException.py
+-rw-rw-rw-   0        0        0      362 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/exceptions/ArgsException.py
+-rw-rw-rw-   0        0        0      396 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/exceptions/CredentialNoBiliJctException.py
+-rw-rw-rw-   0        0        0      390 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/exceptions/CredentialNoBuvid3Exception.py
+-rw-rw-rw-   0        0        0      398 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/exceptions/CredentialNoSessdataException.py
+-rw-rw-rw-   0        0        0      337 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/exceptions/DanmakuClosedException.py
+-rw-rw-rw-   0        0        0      355 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/exceptions/DynamicExceedImagesException.py
+-rw-rw-rw-   0        0        0      220 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/exceptions/LiveException.py
+-rw-rw-rw-   0        0        0      555 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/exceptions/NetworkException.py
+-rw-rw-rw-   0        0        0      727 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/exceptions/ResponseCodeException.py
+-rw-rw-rw-   0        0        0      378 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/exceptions/ResponseException.py
+-rw-rw-rw-   0        0        0      388 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/exceptions/VideoUploadException.py
+-rw-rw-rw-   0        0        0      331 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/exceptions/__init__.py
+-rw-rw-rw-   0        0        0    11478 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/favorite_list.py
+-rw-rw-rw-   0        0        0     3415 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/interactive_video.py
+-rw-rw-rw-   0        0        0    37485 2022-04-27 12:09:52.000000 bilibili-api-python-9.3.1/bilibili_api/live.py
+-rw-rw-rw-   0        0        0     1043 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/misc.py
+-rw-rw-rw-   0        0        0      102 2022-05-05 03:22:03.000000 bilibili-api-python-9.3.1/bilibili_api/settings.py
+-rw-rw-rw-   0        0        0    19151 2022-05-09 02:22:39.000000 bilibili-api-python-9.3.1/bilibili_api/user.py
+drwxrwxrwx   0        0        0        0 2022-05-09 03:14:54.265329 bilibili-api-python-9.3.1/bilibili_api/utils/
+-rw-rw-rw-   0        0        0     2164 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/utils/AsyncEvent.py
+-rw-rw-rw-   0        0        0     5134 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/utils/BytesReader.py
+-rw-rw-rw-   0        0        0     2292 2022-04-27 12:09:52.000000 bilibili-api-python-9.3.1/bilibili_api/utils/Credential.py
+-rw-rw-rw-   0        0        0     3214 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/utils/Danmaku.py
+-rw-rw-rw-   0        0        0        0 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/utils/__init__.py
+-rw-rw-rw-   0        0        0     1258 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/utils/aid_bvid_transformer.py
+-rw-rw-rw-   0        0        0     5557 2022-05-07 10:39:14.000000 bilibili-api-python-9.3.1/bilibili_api/utils/network.py
+-rw-rw-rw-   0        0        0      586 2022-04-27 12:09:52.000000 bilibili-api-python-9.3.1/bilibili_api/utils/sync.py
+-rw-rw-rw-   0        0        0     4173 2022-04-27 12:09:52.000000 bilibili-api-python-9.3.1/bilibili_api/utils/utils.py
+-rw-rw-rw-   0        0        0      598 2022-04-26 08:22:29.000000 bilibili-api-python-9.3.1/bilibili_api/utils/varint.py
+-rw-rw-rw-   0        0        0    45752 2022-05-07 03:03:56.000000 bilibili-api-python-9.3.1/bilibili_api/video.py
+-rw-rw-rw-   0        0        0    24110 2022-04-27 12:09:52.000000 bilibili-api-python-9.3.1/bilibili_api/video_uploader.py
+drwxrwxrwx   0        0        0        0 2022-05-09 03:14:54.286322 bilibili-api-python-9.3.1/bilibili_api_python.egg-info/
+-rw-rw-rw-   0        0        0     6766 2022-05-09 03:14:53.000000 bilibili-api-python-9.3.1/bilibili_api_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2126 2022-05-09 03:14:54.000000 bilibili-api-python-9.3.1/bilibili_api_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-05-09 03:14:53.000000 bilibili-api-python-9.3.1/bilibili_api_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2022-05-09 03:14:53.000000 bilibili-api-python-9.3.1/bilibili_api_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2022-05-09 03:14:53.000000 bilibili-api-python-9.3.1/bilibili_api_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-05-09 03:14:54.293326 bilibili-api-python-9.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1282 2022-05-09 02:22:39.000000 bilibili-api-python-9.3.1/setup.py
```

### Comparing `bilibili-api-python-9.3.0/LICENSE` & `bilibili-api-python-9.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/PKG-INFO` & `bilibili-api-python-9.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bilibili-api-python
-Version: 9.3.0
+Version: 9.3.1
 Summary: 哔哩哔哩的各种 API 调用便捷整合（视频、动态、直播等），另外附加一些常用的功能。
 Home-page: https://github.com/Nemo2011/bilibili_api
 Author: MoyuScript, Nemo2011
 License: GPLv3+
 Keywords: bilibili,api,spider
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `bilibili-api-python-9.3.0/README.md` & `bilibili-api-python-9.3.1/README.md`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/app.py` & `bilibili-api-python-9.3.1/bilibili_api/app.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/article.py` & `bilibili-api-python-9.3.1/bilibili_api/article.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/audio.py` & `bilibili-api-python-9.3.1/bilibili_api/audio.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/bangumi.py` & `bilibili-api-python-9.3.1/bilibili_api/bangumi.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/channel.py` & `bilibili-api-python-9.3.1/bilibili_api/channel.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/comment.py` & `bilibili-api-python-9.3.1/bilibili_api/comment.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/data/api/app.json` & `bilibili-api-python-9.3.1/bilibili_api/data/api/app.json`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/data/api/article.json` & `bilibili-api-python-9.3.1/bilibili_api/data/api/article.json`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/data/api/audio.json` & `bilibili-api-python-9.3.1/bilibili_api/data/api/audio.json`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/data/api/bangumi.json` & `bilibili-api-python-9.3.1/bilibili_api/data/api/bangumi.json`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/data/api/common.json` & `bilibili-api-python-9.3.1/bilibili_api/data/api/common.json`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/data/api/dynamic.json` & `bilibili-api-python-9.3.1/bilibili_api/data/api/dynamic.json`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/data/api/favorite-list.json` & `bilibili-api-python-9.3.1/bilibili_api/data/api/favorite-list.json`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/data/api/interactive_video.json` & `bilibili-api-python-9.3.1/bilibili_api/data/api/interactive_video.json`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/data/api/live.json` & `bilibili-api-python-9.3.1/bilibili_api/data/api/live.json`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/data/api/misc.json` & `bilibili-api-python-9.3.1/bilibili_api/data/api/misc.json`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/data/api/user.json` & `bilibili-api-python-9.3.1/bilibili_api/data/api/user.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.623070987654321%*

 * *Differences: {"'info'": "{'channel_list': {'url': "*

 * *           "'http://api.bilibili.com/x/polymer/space/seasons_series_list', 'params': {'page_num': "*

 * *           "'int: 开始项', 'page_size': 'int: 开始项后面的项数'}, 'comment': '查看用户合集的列表（新版）', 'verity': True, "*

 * *           "delete: ['verify']}, 'channel_video_series': OrderedDict([('url', "*

 * *           "'http://api.bilibili.com/x/series/archives'), ('method', 'GET'), ('verity', True), "*

 * *           "('params', OrderedDict([('mid', 'int: uid'), ('series_id', 'int: series_id'), ('pn' […]*

```diff
@@ -42,42 +42,69 @@
                 "ps": "const int: 15",
                 "type": "int: 1 \u8ffd\u756a\uff0c2 \u8ffd\u5267",
                 "vmid": "int: uid"
             },
             "url": "https://api.bilibili.com/x/space/bangumi/follow/list",
             "verify": false
         },
-        "channel": {
-            "comment": "\u67e5\u770b\u90e8\u5206\u7528\u6237\u7684\u5408\u96c6\u548c\u5217\u8868\u53ca\u90e8\u5206\u5185\u5bb9",
+        "channel_list": {
+            "comment": "\u67e5\u770b\u7528\u6237\u5408\u96c6\u7684\u5217\u8868\uff08\u65b0\u7248\uff09",
             "method": "GET",
             "params": {
-                "mid": "int: uid"
+                "mid": "int: uid",
+                "page_num": "int: \u5f00\u59cb\u9879",
+                "page_size": "int: \u5f00\u59cb\u9879\u540e\u9762\u7684\u9879\u6570"
             },
-            "url": "https://api.bilibili.com/x/space/channel/index",
-            "verify": true
+            "url": "http://api.bilibili.com/x/polymer/space/seasons_series_list",
+            "verity": true
         },
-        "channel_list": {
-            "comment": "\u67e5\u770b\u7528\u6237\u5408\u96c6\u548c\u5217\u8868",
+        "channel_video_season": {
+            "comment": "\u67e5\u770b\u7528\u6237\u5408\u96c6\u4e2d\u7684\u89c6\u9891\uff08\u65b0\u7248\uff09",
             "method": "GET",
             "params": {
-                "mid": "int: uid"
+                "mid": "int: uid",
+                "page_num": "int: \u9875\u7801",
+                "page_size": "int: \u6bcf\u4e00\u9875\u7684\u9879\u6570",
+                "season_id": "int: media_id",
+                "sort_reverse": "bool: \u662f\u5426\u5347\u5e8f\u6392\u5e8f\uff0c\u5426\u5219\u9ed8\u8ba4\u6392\u5e8f"
             },
-            "url": "https://api.bilibili.com/x/space/channel/list",
-            "verify": true
+            "url": "http://api.bilibili.com/x/polymer/space/seasons_archives_list",
+            "verity": true
         },
-        "channel_video": {
-            "comment": "\u67e5\u770b\u5217\u8868\u5185\u89c6\u9891",
+        "channel_video_series": {
+            "comment": "\u67e5\u770b\u5217\u8868\u5185\u89c6\u9891\uff08\u65e7\u7248\uff09",
             "method": "GET",
             "params": {
-                "cid": "int: cid",
                 "mid": "int: uid",
                 "pn": "int: \u9875\u7801",
-                "ps": "const int: 100"
+                "ps": "const int: 100",
+                "series_id": "int: series_id"
             },
-            "url": "https://api.bilibili.com/x/space/channel/video",
+            "url": "http://api.bilibili.com/x/series/archives",
+            "verity": true
+        },
+        "del_channel_aids_series": {
+            "method": "POST",
+            "params": {
+                "aids": "int: aid \u5217\u8868",
+                "mid": "int: uid",
+                "series_id": "int: series_id"
+            },
+            "url": "https://api.bilibili.com/x/series/series/delArchives",
+            "verity": true
+        },
+        "del_channel_series": {
+            "method": "POST",
+            "query": {
+                "aids": "list: \u6240\u6709 aid \u5217\u8868",
+                "csrf": "string: bili_jct \u7684\u503c",
+                "mid": "int: uid",
+                "series_id": "int: series_id"
+            },
+            "url": "https://api.bilibili.com/x/series/series/delete",
             "verity": true
         },
         "dynamic": {
             "comment": "\u7528\u6237\u52a8\u6001\u4fe1\u606f",
             "method": "GET",
             "params": {
                 "host_uid": "int: uid",
@@ -200,40 +227,14 @@
                 "ps": "const int: 30",
                 "tid": "int: \u5206\u533a ID\uff0c0 \u8868\u793a\u5168\u90e8"
             },
             "url": "https://api.bilibili.com/x/space/arc/search",
             "verify": false
         }
     },
-    "new_channel": {
-        "channel_info": {
-            "comment": "\u67e5\u770b\u7528\u6237\u5408\u96c6\u7684\u5217\u8868\uff08\u65b0\u7248\uff09",
-            "method": "GET",
-            "params": {
-                "mid": "int: uid",
-                "page_num": "int: \u5f00\u59cb\u9879",
-                "page_size": "int: \u5f00\u59cb\u9879\u540e\u9762\u7684\u9879\u6570"
-            },
-            "url": "http://api.bilibili.com/x/polymer/space/seasons_series_list",
-            "verity": true
-        },
-        "channel_video": {
-            "comment": "\u67e5\u770b\u7528\u6237\u5408\u96c6\u4e2d\u7684\u89c6\u9891\uff08\u65b0\u7248\uff09",
-            "method": "GET",
-            "params": {
-                "mid": "int: uid",
-                "page_num": "int: \u9875\u7801",
-                "page_size": "int: \u6bcf\u4e00\u9875\u7684\u9879\u6570",
-                "season_id": "int: media_id",
-                "sort_reverse": "bool: \u662f\u5426\u5347\u5e8f\u6392\u5e8f\uff0c\u5426\u5219\u9ed8\u8ba4\u6392\u5e8f"
-            },
-            "url": "http://api.bilibili.com/x/polymer/space/seasons_archives_list",
-            "verity": true
-        }
-    },
     "operate": {
         "create_subscribe_group": {
             "comment": "\u6dfb\u52a0\u5173\u6ce8\u5206\u7ec4",
             "data": {
                 "tag": "str: \u5206\u7ec4\u540d"
             },
             "method": "POST",
```

### Comparing `bilibili-api-python-9.3.0/bilibili_api/data/api/video.json` & `bilibili-api-python-9.3.1/bilibili_api/data/api/video.json`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/data/api/video_uploader.json` & `bilibili-api-python-9.3.1/bilibili_api/data/api/video_uploader.json`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/data/channel.json` & `bilibili-api-python-9.3.1/bilibili_api/data/channel.json`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/dynamic.py` & `bilibili-api-python-9.3.1/bilibili_api/dynamic.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/exceptions/NetworkException.py` & `bilibili-api-python-9.3.1/bilibili_api/exceptions/NetworkException.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/exceptions/ResponseCodeException.py` & `bilibili-api-python-9.3.1/bilibili_api/exceptions/ResponseCodeException.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/favorite_list.py` & `bilibili-api-python-9.3.1/bilibili_api/favorite_list.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/interactive_video.py` & `bilibili-api-python-9.3.1/bilibili_api/interactive_video.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/live.py` & `bilibili-api-python-9.3.1/bilibili_api/live.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/misc.py` & `bilibili-api-python-9.3.1/bilibili_api/misc.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/user.py` & `bilibili-api-python-9.3.1/bilibili_api/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,22 @@
     + FAVORATE: 收藏量倒序。
     + VIEW    : 播放量倒序。
     """
     PUBDATE = "pubdate"
     FAVORATE = "stow"
     VIEW = "click"
 
+class ChannelOrder(Enum):
+    """
+    合集视频排序顺序。
+    + DEFAULT: 默认排序
+    + CHANGE : 升序排序
+    """
+    DEFAULT = "false"
+    CHANGE = "true"
 
 class AudioOrder(Enum):
     """
     音频排序顺序。
 
     + PUBDATE : 上传日期倒序。
     + FAVORATE: 收藏量倒序。
@@ -62,15 +70,14 @@
 
     + LATEST: 最近更新倒序。
     + VIEW  : 总阅读量倒序。
     """
     LATEST = 0
     VIEW = 1
 
-
 class BangumiType(Enum):
     """
     番剧类型。
 
     + BANGUMI: 番剧。
     + DRAMA  : 电视剧/纪录片等。
     """
@@ -180,75 +187,79 @@
             "mid": self.uid
         }
         return await request("GET", url=api["url"], params=params, credential=self.credential)
 
     async def get_videos(self,
                          tid: int = 0,
                          pn: int = 1,
+                         ps: int = 30,
                          keyword: str = "",
                          order: VideoOrder = VideoOrder.PUBDATE
                          ):
         """
         获取用户投稿视频信息。
 
         Args:
             tid     (int, optional)       : 分区 ID. Defaults to 0（全部）.
             pn      (int, optional)       : 页码，从 1 开始. Defaults to 1.
+            ps      (int, optional)       : 每一页的视频数. Defaults to 30. 
             keyword (str, optional)       : 搜索关键词. Defaults to "".
             order   (VideoOrder, optional): 排序方式. Defaults to VideoOrder.PUBDATE
 
         Returns:
             dict.
         """
         api = API["info"]["video"]
         params = {
             "mid": self.uid,
-            "ps": 30,
+            "ps": ps,
             "tid": tid,
             "pn": pn,
             "keyword": keyword,
             "order": order.value
         }
         return await request("GET", url=api["url"], params=params, credential=self.credential)
 
-    async def get_audios(self, order: AudioOrder = AudioOrder.PUBDATE, pn: int = 1):
+    async def get_audios(self, order: AudioOrder = AudioOrder.PUBDATE, pn: int = 1, ps: int = 30):
         """
         获取用户投稿音频。
 
         Args:
             order (AudioOrder, optional): 排序方式. Defaults to AudioOrder.PUBDATE.
             pn    (int, optional)       : 页码数，从 1 开始。 Defaults to 1.
+            ps      (int, optional)       : 每一页的视频数. Defaults to 30. 
 
         Returns:
             dict: 调用接口返回的内容。
         """
         api = API["info"]["audio"]
         params = {
             "uid": self.uid,
-            "ps": 30,
+            "ps": ps,
             "pn": pn,
             "order": order.value
         }
         return await request("GET", url=api["url"], params=params, credential=self.credential)
 
-    async def get_articles(self, pn: int = 1, order: ArticleOrder = ArticleOrder.PUBDATE):
+    async def get_articles(self, pn: int = 1, order: ArticleOrder = ArticleOrder.PUBDATE, ps: int = 30):
         """
         获取用户投稿专栏。
 
         Args:
             order (ArticleOrder, optional): 排序方式. Defaults to ArticleOrder.PUBDATE.
             pn    (int, optional)         : 页码数，从 1 开始。 Defaults to 1.
+            ps      (int, optional)       : 每一页的视频数. Defaults to 30. 
 
         Returns:
             dict: 调用接口返回的内容。
         """
         api = API["info"]["article"]
         params = {
             "mid": self.uid,
-            "ps": 30,
+            "ps": ps,
             "pn": pn,
             "sort": order.value
         }
         return await request("GET", url=api["url"], params=params, credential=self.credential)
 
     async def get_article_list(self, order: ArticleListOrder = ArticleListOrder.LATEST):
         """
@@ -425,91 +436,66 @@
             "msg[timestamp]": int(time.time()),
             "from_filework": 0,
             "build": 0,
             "mobi_app": "web"
         }
         return await request("POST", url=api["url"], data=data, credential=self.credential)
 
-    async def get_channel_old(self):
-        """
-        查看用户部分的合集和列表及部分内容。（旧版）
-
-        Returns:
-            dict: 调用接口返回的内容
-        """
-        api = API["info"]["channel"]
-        param = {
-            "mid": self.uid
-        }
-        return await request("GET", url=api["url"], params=param, credential=self.credential)
-
-    async def get_channel_list_series(self):
-        """
-        查看用户合集和列表。仅供 series_list。
-
-        Returns: 
-            dict: 调用接口返回的内容
-        """
-        api = API["info"]["channel_list"]
-        param = {
-            "mid": self.uid
-        }
-        return await request("GET", url=api["url"], params=param, credential=self.credential)
-
-    async def get_channel_videos_series(self, cid: int, pn: int=1, ps: int=100):
+    async def get_channel_videos_series(self, sid: int, pn: int=1, ps: int=100):
         """
         查看频道内所有视频。仅供 series_list。
 
         Args:
-            cid: 频道的 cid
+            sid: 频道的 series_id
             pn: 页数，默认为 1
             ps: 每一页显示的视频数量
 
         Returns: 
             dict: 调用接口返回的内容
         """
-        api = API["info"]["channel_video"]
+        api = API["info"]["channel_video_series"]
         param = {
             "mid": self.uid,
-            "cid": cid,
+            "series_id": sid,
             "pn": pn,
             "ps": ps
         }
         return await request("GET", url=api["url"], params=param, credential=self.credential)
 
-    async def get_channel_videos_season(self, sid: int, pn: int=1, ps: int=100):
+    async def get_channel_videos_season(self, sid: int, sort: ChannelOrder=ChannelOrder.DEFAULT, pn: int=1, ps: int=100):
         """
         查看频道内所有视频。仅供 season_list。
 
         Args:
-            sid: 频道的 season_id
+            sid: 频道的 media_id
             pn: 页数，默认为 1
             ps: 每一页显示的视频数量
 
         Returns: 
             dict: 调用接口返回的内容
         """
-        api = API["new_channel"]["channel_video"]
+        api = API["info"]["channel_video_season"]
         param = {
             "mid": self.uid,
             "season_id": sid,
-            "pn": pn,
-            "ps": ps
+            "sort_reverse": sort.value,
+            "page_num": pn,
+            "page_size": ps
         }
         return await request("GET", url=api["url"], params=param, credential=self.credential)
 
     async def get_channel_list(self):
         """
         查看用户所有的频道（包括新版）和部分视频。
         适用于获取列表。
 
         Returns:
             dict: 调用接口返回的结果
         """
-        api = API["new_channel"]["channel_info"]
+        api = API["info"]["channel_list"]
         param = {
             "mid": self.uid, 
             "page_num": 1, 
             "page_size": 1
         }
         res = await request("GET", url=api["url"], params=param, credential=self.credential)
         items = res["items_lists"]["page"]["total"]
```

### Comparing `bilibili-api-python-9.3.0/bilibili_api/utils/AsyncEvent.py` & `bilibili-api-python-9.3.1/bilibili_api/utils/AsyncEvent.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/utils/BytesReader.py` & `bilibili-api-python-9.3.1/bilibili_api/utils/BytesReader.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/utils/Credential.py` & `bilibili-api-python-9.3.1/bilibili_api/utils/Credential.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/utils/Danmaku.py` & `bilibili-api-python-9.3.1/bilibili_api/utils/Danmaku.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/utils/aid_bvid_transformer.py` & `bilibili-api-python-9.3.1/bilibili_api/utils/aid_bvid_transformer.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/utils/network.py` & `bilibili-api-python-9.3.1/bilibili_api/utils/network.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/utils/sync.py` & `bilibili-api-python-9.3.1/bilibili_api/utils/sync.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/utils/utils.py` & `bilibili-api-python-9.3.1/bilibili_api/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/utils/varint.py` & `bilibili-api-python-9.3.1/bilibili_api/utils/varint.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/video.py` & `bilibili-api-python-9.3.1/bilibili_api/video.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api/video_uploader.py` & `bilibili-api-python-9.3.1/bilibili_api/video_uploader.py`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/bilibili_api_python.egg-info/PKG-INFO` & `bilibili-api-python-9.3.1/bilibili_api_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bilibili-api-python
-Version: 9.3.0
+Version: 9.3.1
 Summary: 哔哩哔哩的各种 API 调用便捷整合（视频、动态、直播等），另外附加一些常用的功能。
 Home-page: https://github.com/Nemo2011/bilibili_api
 Author: MoyuScript, Nemo2011
 License: GPLv3+
 Keywords: bilibili,api,spider
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `bilibili-api-python-9.3.0/bilibili_api_python.egg-info/SOURCES.txt` & `bilibili-api-python-9.3.1/bilibili_api_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bilibili-api-python-9.3.0/setup.py` & `bilibili-api-python-9.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r", encoding="utf8") as f:
     requires = f.read()
 
 setuptools.setup(
     name='bilibili-api-python',
-    version='9.3.0',
+    version='9.3.1',
     license='GPLv3+',
     author='MoyuScript, Nemo2011',
     description='哔哩哔哩的各种 API 调用便捷整合（视频、动态、直播等），另外附加一些常用的功能。',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["tests"]),
     keywords=[
```

