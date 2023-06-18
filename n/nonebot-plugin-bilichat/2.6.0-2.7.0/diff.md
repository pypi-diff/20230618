# Comparing `tmp/nonebot_plugin_bilichat-2.6.0.tar.gz` & `tmp/nonebot_plugin_bilichat-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-2.6.0.tar", last modified: Fri Jun 16 16:28:16 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-2.7.0.tar", last modified: Sun Jun 18 17:38:28 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-2.6.0.tar` & `nonebot_plugin_bilichat-2.7.0.tar`

### file list

```diff
@@ -1,31 +1,36 @@
--rw-r--r--   0        0        0    34523 2023-06-16 16:28:08.131567 nonebot_plugin_bilichat-2.6.0/LICENSE
--rw-r--r--   0        0        0    12661 2023-06-16 16:28:08.131567 nonebot_plugin_bilichat-2.6.0/README.md
--rw-r--r--   0        0        0     9278 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4914 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      871 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6463 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0    11820 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3812 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      555 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0      503 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0    27359 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/model/newbing.py
--rw-r--r--   0        0        0      323 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1363 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     6899 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4916 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2363 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1780 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1499 2023-06-16 16:28:16.331509 nonebot_plugin_bilichat-2.6.0/pyproject.toml
--rw-r--r--   0        0        0    14102 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-18 17:38:19.335756 nonebot_plugin_bilichat-2.7.0/LICENSE
+-rw-r--r--   0        0        0    13119 2023-06-18 17:38:19.335756 nonebot_plugin_bilichat-2.7.0/README.md
+-rw-r--r--   0        0        0     9452 2023-06-18 17:38:19.355756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     5512 2023-06-18 17:38:19.355756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-06-18 17:38:19.355756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-06-18 17:38:19.355756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-06-18 17:38:19.355756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      871 2023-06-18 17:38:19.355756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6502 2023-06-18 17:38:19.359756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0    15455 2023-06-18 17:38:19.359756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3812 2023-06-18 17:38:19.359756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      555 2023-06-18 17:38:19.359756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-06-18 17:38:19.359756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-06-18 17:38:19.359756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-06-18 17:38:19.359756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-06-18 17:38:19.359756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-06-18 17:38:19.359756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-06-18 17:38:19.359756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      503 2023-06-18 17:38:19.359756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0    27359 2023-06-18 17:38:19.359756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-06-18 17:38:19.359756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-06-18 17:38:19.359756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-06-18 17:38:19.359756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1187 2023-06-18 17:38:19.359756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png
+-rw-r--r--   0        0        0     1200 2023-06-18 17:38:19.359756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
+-rw-r--r--   0        0        0    14952 2023-06-18 17:38:19.359756 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/static/style_blue/assets/vanfont.ttf
+-rw-r--r--   0        0        0    93905 2023-06-18 17:38:19.363757 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
+-rw-r--r--   0        0        0     7114 2023-06-18 17:38:19.363757 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/static/style_blue/video-details.html
+-rw-r--r--   0        0        0     1363 2023-06-18 17:38:19.363757 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     6899 2023-06-18 17:38:19.363757 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4916 2023-06-18 17:38:19.363757 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2363 2023-06-18 17:38:19.363757 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-06-18 17:38:19.363757 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1780 2023-06-18 17:38:19.363757 nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1583 2023-06-18 17:38:28.764019 nonebot_plugin_bilichat-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0    14694 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.7.0/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-2.6.0/LICENSE` & `nonebot_plugin_bilichat-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.6.0/README.md` & `nonebot_plugin_bilichat-2.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -162,17 +162,32 @@
 3. `bilichat_dynamic_font` 可填写自定义的字体url，但并不推荐修改
 4. 当使用 `bcut_asr` 接口来生成AI字幕时，根据视频时长和网络情况有可能会识别失败，Bot会提示 `BCut-ASR conversion failed due to network error`。可以通过调高 `bilichat_neterror_retry` 次数或几分钟后重试来尝试重新生成字幕
 
 ### 基础信息配置项
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| bilichat_basic_info          | bool | True | 是否开启视频基本信息 |
-| bilichat_basic_info_url      | bool | True | 开启视频进本信息的情况下，是否一同回复一个链接 |
-| bilichat_reply_to_basic_info | bool | True | 后续消息是否回复基础信息(关闭则回复发送者的信息) |
+| bilichat_basic_info          | bool | True         | 是否开启视频基本信息 |
+| bilichat_basic_info_style    | str  | bbot_default | 视频详情的图片样式，可用样式见下方备注 |
+| bilichat_basic_info_url      | bool | True         | 开启视频进本信息的情况下，是否一同回复一个链接 |
+| bilichat_reply_to_basic_info | bool | True         | 后续消息是否回复基础信息(关闭则回复发送者的信息) |
+
+注：bilichat_basic_info_style 除默认的 bbot_default 使用 PIL 绘图，其他均依赖于 `nonebot-plugin-htmlrender`，其可用的样式如下所示
+
+<details>
+<summary>bbot_default</summary>
+
+![](docs/bbot_default.png)
+</details>
+
+<details>
+<summary>style_blue</summary>
+
+![](docs/style_blue.png)
+</details>
 
 ### 词云配置项
 
 开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[wordcloud]`
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
```

#### html2text {}

```diff
@@ -55,27 +55,32 @@
 å¯å¡«åèªå®ä¹çå­ä½urlï¼ä½å¹¶ä¸æ¨èä¿®æ¹ 4. å½ä½¿ç¨ `bcut_asr`
 æ¥å£æ¥çæAIå­å¹æ¶ï¼æ ¹æ®è§é¢æ¶é¿åç½ç»æåµæå¯è½ä¼è¯å«å¤±è´¥ï¼Botä¼æç¤º
 `BCut-ASR conversion failed due to network error`ãå¯ä»¥éè¿è°é«
 `bilichat_neterror_retry`
 æ¬¡æ°æå åéåéè¯æ¥å°è¯éæ°çæå­å¹ ###
 åºç¡ä¿¡æ¯éç½®é¡¹ | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:---
 -:|:----:|:----:| | bilichat_basic_info | bool | True |
-æ¯å¦å¼å¯è§é¢åºæ¬ä¿¡æ¯ | | bilichat_basic_info_url | bool | True |
+æ¯å¦å¼å¯è§é¢åºæ¬ä¿¡æ¯ | | bilichat_basic_info_style | str |
+bbot_default | è§é¢è¯¦æçå¾çæ ·å¼ï¼å¯ç¨æ ·å¼è§ä¸æ¹å¤æ³¨ | |
+bilichat_basic_info_url | bool | True |
 å¼å¯è§é¢è¿æ¬ä¿¡æ¯çæåµä¸ï¼æ¯å¦ä¸ååå¤ä¸ä¸ªé¾æ¥ | |
 bilichat_reply_to_basic_info | bool | True |
-åç»­æ¶æ¯æ¯å¦åå¤åºç¡ä¿¡æ¯(å³é­ååå¤åéèçä¿¡æ¯) | ###
-è¯äºéç½®é¡¹ å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-
-bilichat[wordcloud]` | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:---
--:|:----:|:----:| | bilichat_word_cloud | bool | True |
-æ¯å¦å¼å¯è¯äºåè½ | æ³¨ï¼è¯äºåè½å¨ python3.11 ä¸­ç±äº
-`wordcloud` åå®è£å¤±è´¥ææ¶æ æ³å¯ç¨ï¼è¯·ä¸è¦å¨ 3.11
-ä¸­å¼å¯æ­¤åè½ ### AIè§é¢æ»ç»éç½®é¡¹
-å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-bilichat
-[openai,newbing]` | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:
-----:|:----:| | bilichat_newbing_cookie | str | None |
+åç»­æ¶æ¯æ¯å¦åå¤åºç¡ä¿¡æ¯(å³é­ååå¤åéèçä¿¡æ¯) |
+æ³¨ï¼bilichat_basic_info_style é¤é»è®¤ç bbot_default ä½¿ç¨ PIL
+ç»å¾ï¼å¶ä»åä¾èµäº `nonebot-plugin-
+htmlrender`ï¼å¶å¯ç¨çæ ·å¼å¦ä¸æç¤º  bbot_default ![](docs/
+bbot_default.png)   style_blue ![](docs/style_blue.png)  ### è¯äºéç½®é¡¹
+å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-bilichat[wordcloud]`
+| éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| |
+bilichat_word_cloud | bool | True | æ¯å¦å¼å¯è¯äºåè½ |
+æ³¨ï¼è¯äºåè½å¨ python3.11 ä¸­ç±äº `wordcloud`
+åå®è£å¤±è´¥ææ¶æ æ³å¯ç¨ï¼è¯·ä¸è¦å¨ 3.11 ä¸­å¼å¯æ­¤åè½ ###
+AIè§é¢æ»ç»éç½®é¡¹ å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-
+plugin-bilichat[openai,newbing]` | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:
+-----:|:----:|:----:|:----:| | bilichat_newbing_cookie | str | None |
 newbingçcookieæä»¶è·¯å¾, å¡«å `no_login`
 åä¸è¿è¡ç»å½ï¼å¯è½ææ¬¡æ°éå¶ï¼, è¥çç©ºåç¦ç¨newbingæ»ç»
 | | bilichat_newbing_token_limit | int | 0 | newbingè¯·æ±çææ¬éä¸é,
 0ä¸ºæ ä¸é | | bilichat_newbing_preprocess | bool | True |
 æ¯å¦å¯¹newbingçè¿åå¼è¿è¡é¢å¤ç, ä»¥å»é¤å¶ä¸­ä¸æ³è¦çåå®¹
 | | bilichat_openai_token | str | None | openaiçapikey,
 è¥çç©ºåç¦ç¨openaiæ»ç» | | bilichat_openai_proxy | str | None |
```

### Comparing `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,18 +166,23 @@
     DISABLE_LINK = isinstance(bot, QG_Bot) or not plugin_config.bilichat_basic_info_url  # 部分平台发送链接都要审核
     SEND_IMAGE_SEPARATELY = isinstance(bot, QG_Bot)  # 部分平台无法一次性发送多张图片，或无法与其他消息组合发出
     reply = "" if DISABLE_REPLY else await SegmentBuilder.reply()
     # basic info
     bili_number, uid = state["bili_number"], state["_uid_"]
     if bili_number[:2] in ["BV", "bv", "av"]:
         msg, img, info = await get_video_basic(bili_number, uid)
-        if not msg or not info:
+        # 检查视频是否包含有效信息
+        if not (msg and info):
+            if msg:
+                await matcher.finish(reply + msg)
             raise FinishedException
+        # 如果不含图片
         if not img:
             await matcher.finish(reply + msg)
+        # 如果包含图片
         elif img != "IMG_RENDER_DISABLED":
             image = await SegmentBuilder.image(image=img)
             msg = "" if DISABLE_LINK else msg
             if SEND_IMAGE_SEPARATELY:
                 if reply and msg:
                     await matcher.send(reply + msg)
                 re_msg = await matcher.send(image)
```

### Comparing `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import importlib.util
 import json
 import sys
 from pathlib import Path
 from typing import List, Literal, Optional, Union
 
-from nonebot import get_driver
+from nonebot import get_driver, require
 from nonebot.log import logger
 from pydantic import BaseModel, validator
 
 # get package version
 if sys.version_info < (3, 10):
     from importlib_metadata import version
 else:
@@ -33,14 +33,15 @@
     bilichat_dynamic_font: Optional[str]
     bilichat_cd_time: int = 120
     bilichat_neterror_retry: int = 3
     bilichat_show_error_msg: bool = True
 
     # basic info
     bilichat_basic_info: bool = True
+    bilichat_basic_info_style: Literal["bbot_default", "style_blue"] = "bbot_default"
     bilichat_basic_info_url: bool = True
     bilichat_reply_to_basic_info: bool = True
 
     # both WC and AI
     bilichat_use_bcut_asr: bool = True
 
     # Word Cloud
@@ -122,14 +123,28 @@
     def check_pypackage_wordcloud(cls, v):
         if (importlib.util.find_spec("wordcloud") and importlib.util.find_spec("jieba")) or not v:
             return v
         else:
             raise RuntimeError(
                 "Package(s) of fuction wordcloud not installed, use **pip install nonebot-plugin-bilichat[wordcloud]** to install required dependencies"
             )
+    
+    @validator("bilichat_basic_info_style",always=True)
+    def check_htmlrender(cls,v):
+        if v == "bbot_default":
+            return v
+        else:
+            try:
+                require("nonebot_plugin_htmlrender")
+                return v
+            except Exception as e:
+                raise RuntimeError(
+                    "Package(s) of fuction styles not installed, use **pip install nonebot-plugin-bilichat[extra]** to install required dependencies"
+                ) from e
+
 
     def verify_permission(self, uid: Union[str, int]):
         if self.bilichat_whitelist:
             return str(uid) in self.bilichat_whitelist
         elif self.bilichat_blacklist:
             return str(uid) not in self.bilichat_blacklist
         else:
```

### Comparing `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     if not check_cd(f"{aid}_{uid}"):
         logger.warning(f"Duplicate video {aid}. Skip the video parsing process")
         return (None, None, None)
     # generate video information
     try:
         b23_url = await get_b23_url(f"https://www.bilibili.com/video/{bvid}")
         data = (
-            (await (await BiliVideoImage.from_view_rely(video_info, b23_url)).render())
+            (await (await BiliVideoImage.from_view_rely(video_info, b23_url)).render(plugin_config.bilichat_basic_info_style))
             if plugin_config.bilichat_basic_info
             else "IMG_RENDER_DISABLED"
         )
         logger.debug(f"Video parsing complete - aid:{aid} cid:{cid} title:{title}")
         return (b23_url, data, Video(aid, cid, title))
     except TimeoutException:
         logger.warning("Video parsing API call timeout")
```

### Comparing `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import asyncio
+import base64
+from datetime import datetime
 from io import BytesIO
+from pathlib import Path
 from typing import List, Optional, Union
 
 import qrcode
 from bilireq.exceptions import ResponseCodeError
 from bilireq.grpc.protos.bilibili.app.view.v1.view_pb2 import ViewReply
 from httpx import AsyncClient
 from PIL import Image, ImageDraw, ImageFont
@@ -21,46 +24,50 @@
 class UP:
     def __init__(
         self,
         name: str,
         face: Union[bytes, BytesIO],
         level: int,
         fans: str,
+        video_counts: int,
         title: str = "UP主",
         name_color: str = "black",
     ) -> None:
         self.name: str = name
         self.face: BytesIO = face if isinstance(face, BytesIO) else BytesIO(face)
         self.level: int = level
         self.name_color: str = name_color or "black"
         self.fans: str = fans
+        self.video_counts: int = video_counts
         self.title: str = title
 
     @classmethod
     async def from_id(cls, client: AsyncClient, mid: int, name: str, title: str):
         try:
             up_data = await get_user_space_info(mid)
         except ResponseCodeError as e:
             if e.code in [-404, 404]:
                 up_data = None
             else:
                 raise e
         bg_color = up_data["card"]["vip"]["label"]["bg_color"] if up_data else "black"
         level = up_data["card"]["level_info"]["current_level"] if up_data else 0
+        video_counts = up_data["archive"]["count"] if up_data else 0
         face_url = up_data["card"]["face"] if up_data else "https://i0.hdslb.com/bfs/face/member/noface.jpg"
         face_req = await client.get(face_url)
         if face_req.status_code == 404:
             face_req = await client.get(f"{face_url}@160w_160h_1c_1s.webp")
         face = face_req.content
         return cls(
             name=name,
             name_color=bg_color,
             level=level,
             face=face,
             fans=num_fmt(up_data["card"]["fans"]) if up_data else "N/A",
+            video_counts=video_counts,
             title=title,
         )
 
 
 class BiliVideoImage:
     def __init__(
         self,
@@ -69,31 +76,39 @@
         type_name: str,
         title: str,
         view: str,
         danmaku: str,
         favorite: str,
         coin: str,
         like: str,
+        reply: str,
+        share: str,
+        pubdate: datetime,
         uploaders: List[UP],
         b23_url: str,
+        aid: str,
         desc: Optional[str] = None,
     ):
-        self.cover: Union[bytes, BytesIO] = cover if isinstance(cover, BytesIO) else BytesIO(cover)
+        self.cover: BytesIO = cover if isinstance(cover, BytesIO) else BytesIO(cover)
         minutes, self.seconds = divmod(duration, 60)
         self.hours, self.minutes = divmod(minutes, 60)
         self.type_name: str = type_name
         self.title: str = title
         self.desc: str = desc or "该视频没有简介"
         self.view: str = view
         self.danmaku: str = danmaku
         self.favorite: str = favorite
         self.coin: str = coin
         self.like: str = like
+        self.reply: str = reply
+        self.share: str = share
+        self.pubdate: datetime = pubdate
         self.uploaders: List[UP] = uploaders
         self.b23_url: str = b23_url
+        self.aid: str = aid
 
     @classmethod
     async def from_view_rely(cls, video_view: ViewReply, b23_url: str) -> "BiliVideoImage":
         video_info = video_view.activity_season if video_view.activity_season.arc.aid else video_view
         # 获取封面
         client = hc
         client.headers.update(
@@ -125,23 +140,53 @@
             title=video_info.arc.title,
             desc=video_info.arc.desc,
             view=num_fmt(video_info.arc.stat.view),
             danmaku=num_fmt(video_info.arc.stat.danmaku),
             favorite=num_fmt(video_info.arc.stat.fav),
             coin=num_fmt(video_info.arc.stat.coin),
             like=num_fmt(video_info.arc.stat.like),
+            reply=num_fmt(video_info.arc.stat.reply),
+            share=num_fmt(video_info.arc.stat.share),
+            pubdate=datetime.fromtimestamp(video_info.arc.pubdate),
             uploaders=ups,
             b23_url=b23_url,
+            aid=f"av{video_info.arc.aid}",
         )
 
+    @staticmethod
+    def get_up_level_code(level: int):
+        if level == 0:
+            up_level = "\uE6CB"
+            level_color = (191, 191, 191)
+        elif level == 1:
+            up_level = "\uE6CC"
+            level_color = (191, 191, 191)
+        elif level == 2:
+            up_level = "\uE6CD"
+            level_color = (149, 221, 178)
+        elif level == 3:
+            up_level = "\uE6CE"
+            level_color = (146, 209, 229)
+        elif level == 4:
+            up_level = "\uE6CF"
+            level_color = (255, 179, 124)
+        elif level == 5:
+            up_level = "\uE6D0"
+            level_color = (255, 108, 0)
+        else:
+            up_level = "\uE6D1"
+            level_color = (255, 0, 0)
+        return up_level, level_color
+
     async def render(self, style: str = "bbot_default"):
         loop = asyncio.get_running_loop()
         if style == "bbot_default":
-            func = self.style_bbot_default
-        return await loop.run_in_executor(None, func) # type: ignore
+            return await loop.run_in_executor(None, self.style_bbot_default)  # type: ignore
+        if style == "style_blue":
+            return await self.style_blue()
 
     def style_bbot_default(self):
         bg_y = 0
         # ===  封面 ===
         ## 封面
         cover = Image.open(self.cover)
         pic = cover.resize((560, 350))
@@ -215,35 +260,15 @@
         mask = Image.new("RGBA", face_size, color=(0, 0, 0, 0))
         mask_draw = ImageDraw.Draw(mask)
         mask_draw.ellipse((0, 0, face_size[0], face_size[1]), fill=(0, 0, 0, 255))
         name_font = ImageFont.truetype(font_bold, 24)
         up_title_font = ImageFont.truetype(font_bold, 20)
         follower_font = ImageFont.truetype(font_semibold, 22)
         for i, up in enumerate(self.uploaders):
-            if up.level == 0:
-                up_level = "\uE6CB"
-                level_color = (191, 191, 191)
-            elif up.level == 1:
-                up_level = "\uE6CC"
-                level_color = (191, 191, 191)
-            elif up.level == 2:
-                up_level = "\uE6CD"
-                level_color = (149, 221, 178)
-            elif up.level == 3:
-                up_level = "\uE6CE"
-                level_color = (146, 209, 229)
-            elif up.level == 4:
-                up_level = "\uE6CF"
-                level_color = (255, 179, 124)
-            elif up.level == 5:
-                up_level = "\uE6D0"
-                level_color = (255, 108, 0)
-            else:
-                up_level = "\uE6D1"
-                level_color = (255, 0, 0)
+            up_level, level_color = self.get_up_level_code(up.level)
             # 头像
             face = Image.open(up.face)
             face.convert("RGB")
             face = face.resize(face_size)
             up_bg.paste(face, (20, 20 + (i * 120)), mask)
             # 名字
             draw.text(
@@ -301,7 +326,76 @@
             banner_bg,
             (0, 390 + title_bg_y + 20 + dynamic_bg_y + 10 + info_bg_y + up_bg_y - 18),
         )
         image = BytesIO()
         video.save(image, "JPEG")
 
         return image.getvalue()
+
+    async def style_blue(self):
+        import jinja2
+        from nonebot_plugin_htmlrender.browser import get_new_page
+
+        style_bule = Path(__file__).parent.parent.joinpath("static", "style_blue")
+        assets = style_bule.joinpath("assets")
+        video_time = (
+            f"{self.hours:02d}:{self.minutes:02d}:{self.seconds:02d}"
+            if self.hours
+            else f"{self.minutes:02d}:{self.seconds:02d}"
+        )
+        qr = qrcode.QRCode(border=1)
+        qr.add_data(self.b23_url)
+        qr_image = BytesIO()
+        qr.make_image(PilImage).save(qr_image, "JPEG")
+
+        ups = []
+        for up in self.uploaders:
+            level, level_color = self.get_up_level_code(up.level)
+            info = {
+                "avatar_image": f"data:image/png;base64,{base64.b64encode(up.face.getvalue()).decode()}",
+                "name": up.name,
+                "level": level,
+                "name_color": up.name_color,
+                "level_color": f"rgba{level_color}",
+                "fans_count": up.fans,
+                "video_count": up.video_counts,
+            }
+            if up.title:
+                info["condition"] = up.title
+            ups.append(info)
+
+        template_env = jinja2.Environment(
+            loader=jinja2.FileSystemLoader(style_bule),
+            enable_async=True,
+        )
+        template_path = f"file:///{style_bule.joinpath('video-details.html').absolute()}".replace("////", "///")
+        template = template_env.get_template("video-details.html")
+        html = await template.render_async(
+            **{
+                "vanfont": f"file:///{font_vanfont}".replace("////", "///"),
+                "cover_image": f"data:image/png;base64,{base64.b64encode(self.cover.getvalue()).decode()}",
+                "video_category": self.type_name,
+                "video_duration": video_time,
+                "up_infos": ups,
+                "video_title": self.title,
+                "view_count": self.view,
+                "dm_count": self.danmaku,
+                "reply_count": self.reply,
+                "upload_date": self.pubdate.strftime("%Y-%m-%d"),
+                "av_number": self.aid,
+                "video_summary": self.desc,
+                "like_count": self.like,
+                "coin_count": self.coin,
+                "fav_count": self.favorite,
+                "share_count": self.share,
+                "qr_code_image": f"data:image/png;base64,{base64.b64encode(qr_image.getvalue()).decode()}",
+            }
+        )
+
+        async with get_new_page() as page:
+            await page.goto(template_path)
+            await page.set_content(html, wait_until="networkidle")
+            await page.wait_for_timeout(5)
+            img_raw = await page.locator(".video").screenshot(
+                type="png",
+            )
+        return img_raw
```

### Comparing `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/store.py` & `nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/lib/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/model/newbing.py` & `nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/model/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-2.7.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.6.0/pyproject.toml` & `nonebot_plugin_bilichat-2.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "2.6.0"
+version = "2.7.0"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.4",
@@ -43,14 +43,15 @@
 
 [project.license]
 text = "AGPL3.0"
 
 [project.optional-dependencies]
 extra = [
     "nonebot-plugin-sentry>=0.2.2",
+    "nonebot-plugin-htmlrender>=0.2.0.3",
 ]
 wordcloud = [
     "jieba>=0.42.1",
     "wordcloud>=1.8.2.2",
 ]
 openai = [
     "tiktoken-async>=0.3.2",
@@ -63,14 +64,15 @@
 ]
 all = [
     "jieba>=0.42.1",
     "wordcloud>=1.8.2.2",
     "tiktoken-async>=0.3.2",
     "EdgeGPT>=0.1.22.1,<0.9.0",
     "minidynamicrender>=1.1.9",
+    "nonebot-plugin-htmlrender>=0.2.0.3",
     "setuptools",
 ]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
```

### Comparing `nonebot_plugin_bilichat-2.6.0/PKG-INFO` & `nonebot_plugin_bilichat-2.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 2.6.0
+Version: 2.7.0
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2
 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot-adapter-onebot>=2.2.2
 Requires-Dist: nonebot-plugin-segbuilder>=0.2.0
 Requires-Dist: nonebot2>=2.0.0
 Requires-Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra"
+Requires-Dist: nonebot-plugin-htmlrender>=0.2.0.3; extra == "extra"
 Requires-Dist: jieba>=0.42.1; extra == "wordcloud"
 Requires-Dist: wordcloud>=1.8.2.2; extra == "wordcloud"
 Requires-Dist: tiktoken-async>=0.3.2; extra == "openai"
 Requires-Dist: minidynamicrender>=1.1.9; extra == "openai"
 Requires-Dist: EdgeGPT<0.9.0,>=0.1.22.1; extra == "newbing"
 Requires-Dist: minidynamicrender>=1.1.9; extra == "newbing"
 Requires-Dist: setuptools; extra == "newbing"
 Requires-Dist: jieba>=0.42.1; extra == "all"
 Requires-Dist: wordcloud>=1.8.2.2; extra == "all"
 Requires-Dist: tiktoken-async>=0.3.2; extra == "all"
 Requires-Dist: EdgeGPT<0.9.0,>=0.1.22.1; extra == "all"
 Requires-Dist: minidynamicrender>=1.1.9; extra == "all"
+Requires-Dist: nonebot-plugin-htmlrender>=0.2.0.3; extra == "all"
 Requires-Dist: setuptools; extra == "all"
 Provides-Extra: extra
 Provides-Extra: wordcloud
 Provides-Extra: openai
 Provides-Extra: newbing
 Provides-Extra: all
 Description-Content-Type: text/markdown
@@ -198,17 +200,32 @@
 3. `bilichat_dynamic_font` 可填写自定义的字体url，但并不推荐修改
 4. 当使用 `bcut_asr` 接口来生成AI字幕时，根据视频时长和网络情况有可能会识别失败，Bot会提示 `BCut-ASR conversion failed due to network error`。可以通过调高 `bilichat_neterror_retry` 次数或几分钟后重试来尝试重新生成字幕
 
 ### 基础信息配置项
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| bilichat_basic_info          | bool | True | 是否开启视频基本信息 |
-| bilichat_basic_info_url      | bool | True | 开启视频进本信息的情况下，是否一同回复一个链接 |
-| bilichat_reply_to_basic_info | bool | True | 后续消息是否回复基础信息(关闭则回复发送者的信息) |
+| bilichat_basic_info          | bool | True         | 是否开启视频基本信息 |
+| bilichat_basic_info_style    | str  | bbot_default | 视频详情的图片样式，可用样式见下方备注 |
+| bilichat_basic_info_url      | bool | True         | 开启视频进本信息的情况下，是否一同回复一个链接 |
+| bilichat_reply_to_basic_info | bool | True         | 后续消息是否回复基础信息(关闭则回复发送者的信息) |
+
+注：bilichat_basic_info_style 除默认的 bbot_default 使用 PIL 绘图，其他均依赖于 `nonebot-plugin-htmlrender`，其可用的样式如下所示
+
+<details>
+<summary>bbot_default</summary>
+
+![](docs/bbot_default.png)
+</details>
+
+<details>
+<summary>style_blue</summary>
+
+![](docs/style_blue.png)
+</details>
 
 ### 词云配置项
 
 开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[wordcloud]`
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
```

#### html2text {}

```diff
@@ -1,26 +1,28 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.6.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.7.0 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-Dist: nonebot-plugin-
 segbuilder>=0.2.0 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-
-sentry>=0.2.2; extra == "extra" Requires-Dist: jieba>=0.42.1; extra ==
+sentry>=0.2.2; extra == "extra" Requires-Dist: nonebot-plugin-
+htmlrender>=0.2.0.3; extra == "extra" Requires-Dist: jieba>=0.42.1; extra ==
 "wordcloud" Requires-Dist: wordcloud>=1.8.2.2; extra == "wordcloud" Requires-
 Dist: tiktoken-async>=0.3.2; extra == "openai" Requires-Dist:
 minidynamicrender>=1.1.9; extra == "openai" Requires-Dist:
 EdgeGPT<0.9.0,>=0.1.22.1; extra == "newbing" Requires-Dist:
 minidynamicrender>=1.1.9; extra == "newbing" Requires-Dist: setuptools; extra
 == "newbing" Requires-Dist: jieba>=0.42.1; extra == "all" Requires-Dist:
 wordcloud>=1.8.2.2; extra == "all" Requires-Dist: tiktoken-async>=0.3.2; extra
 == "all" Requires-Dist: EdgeGPT<0.9.0,>=0.1.22.1; extra == "all" Requires-Dist:
-minidynamicrender>=1.1.9; extra == "all" Requires-Dist: setuptools; extra ==
-"all" Provides-Extra: extra Provides-Extra: wordcloud Provides-Extra: openai
+minidynamicrender>=1.1.9; extra == "all" Requires-Dist: nonebot-plugin-
+htmlrender>=0.2.0.3; extra == "all" Requires-Dist: setuptools; extra == "all"
+Provides-Extra: extra Provides-Extra: wordcloud Provides-Extra: openai
 Provides-Extra: newbing Provides-Extra: all Description-Content-Type: text/
 markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
     # nonebot-plugin-bilichat _â¨ å¤åè½çBç«è§é¢è§£æå·¥å· â¨_
 [license] [PyPI_-_Downloads] [pypi] [python] [pdm-managed] [Code_style:_black]
                [onebot] [onebot] [QQ_Chat_Group] [QQ_Chat_Group]
@@ -76,27 +78,32 @@
 å¯å¡«åèªå®ä¹çå­ä½urlï¼ä½å¹¶ä¸æ¨èä¿®æ¹ 4. å½ä½¿ç¨ `bcut_asr`
 æ¥å£æ¥çæAIå­å¹æ¶ï¼æ ¹æ®è§é¢æ¶é¿åç½ç»æåµæå¯è½ä¼è¯å«å¤±è´¥ï¼Botä¼æç¤º
 `BCut-ASR conversion failed due to network error`ãå¯ä»¥éè¿è°é«
 `bilichat_neterror_retry`
 æ¬¡æ°æå åéåéè¯æ¥å°è¯éæ°çæå­å¹ ###
 åºç¡ä¿¡æ¯éç½®é¡¹ | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:---
 -:|:----:|:----:| | bilichat_basic_info | bool | True |
-æ¯å¦å¼å¯è§é¢åºæ¬ä¿¡æ¯ | | bilichat_basic_info_url | bool | True |
+æ¯å¦å¼å¯è§é¢åºæ¬ä¿¡æ¯ | | bilichat_basic_info_style | str |
+bbot_default | è§é¢è¯¦æçå¾çæ ·å¼ï¼å¯ç¨æ ·å¼è§ä¸æ¹å¤æ³¨ | |
+bilichat_basic_info_url | bool | True |
 å¼å¯è§é¢è¿æ¬ä¿¡æ¯çæåµä¸ï¼æ¯å¦ä¸ååå¤ä¸ä¸ªé¾æ¥ | |
 bilichat_reply_to_basic_info | bool | True |
-åç»­æ¶æ¯æ¯å¦åå¤åºç¡ä¿¡æ¯(å³é­ååå¤åéèçä¿¡æ¯) | ###
-è¯äºéç½®é¡¹ å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-
-bilichat[wordcloud]` | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:---
--:|:----:|:----:| | bilichat_word_cloud | bool | True |
-æ¯å¦å¼å¯è¯äºåè½ | æ³¨ï¼è¯äºåè½å¨ python3.11 ä¸­ç±äº
-`wordcloud` åå®è£å¤±è´¥ææ¶æ æ³å¯ç¨ï¼è¯·ä¸è¦å¨ 3.11
-ä¸­å¼å¯æ­¤åè½ ### AIè§é¢æ»ç»éç½®é¡¹
-å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-bilichat
-[openai,newbing]` | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:
-----:|:----:| | bilichat_newbing_cookie | str | None |
+åç»­æ¶æ¯æ¯å¦åå¤åºç¡ä¿¡æ¯(å³é­ååå¤åéèçä¿¡æ¯) |
+æ³¨ï¼bilichat_basic_info_style é¤é»è®¤ç bbot_default ä½¿ç¨ PIL
+ç»å¾ï¼å¶ä»åä¾èµäº `nonebot-plugin-
+htmlrender`ï¼å¶å¯ç¨çæ ·å¼å¦ä¸æç¤º  bbot_default ![](docs/
+bbot_default.png)   style_blue ![](docs/style_blue.png)  ### è¯äºéç½®é¡¹
+å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-bilichat[wordcloud]`
+| éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| |
+bilichat_word_cloud | bool | True | æ¯å¦å¼å¯è¯äºåè½ |
+æ³¨ï¼è¯äºåè½å¨ python3.11 ä¸­ç±äº `wordcloud`
+åå®è£å¤±è´¥ææ¶æ æ³å¯ç¨ï¼è¯·ä¸è¦å¨ 3.11 ä¸­å¼å¯æ­¤åè½ ###
+AIè§é¢æ»ç»éç½®é¡¹ å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-
+plugin-bilichat[openai,newbing]` | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:
+-----:|:----:|:----:|:----:| | bilichat_newbing_cookie | str | None |
 newbingçcookieæä»¶è·¯å¾, å¡«å `no_login`
 åä¸è¿è¡ç»å½ï¼å¯è½ææ¬¡æ°éå¶ï¼, è¥çç©ºåç¦ç¨newbingæ»ç»
 | | bilichat_newbing_token_limit | int | 0 | newbingè¯·æ±çææ¬éä¸é,
 0ä¸ºæ ä¸é | | bilichat_newbing_preprocess | bool | True |
 æ¯å¦å¯¹newbingçè¿åå¼è¿è¡é¢å¤ç, ä»¥å»é¤å¶ä¸­ä¸æ³è¦çåå®¹
 | | bilichat_openai_token | str | None | openaiçapikey,
 è¥çç©ºåç¦ç¨openaiæ»ç» | | bilichat_openai_proxy | str | None |
```

