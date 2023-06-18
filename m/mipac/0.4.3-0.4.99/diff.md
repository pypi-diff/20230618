# Comparing `tmp/mipac-0.4.3.tar.gz` & `tmp/mipac-0.4.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mipac-0.4.3.tar", last modified: Tue Apr 25 08:41:27 2023, max compression
+gzip compressed data, was "mipac-0.4.99.tar", last modified: Sun Jun 18 02:31:40 2023, max compression
```

## Comparing `mipac-0.4.3.tar` & `mipac-0.4.99.tar`

### file list

```diff
@@ -1,146 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.529852 mipac-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-25 08:41:11.000000 mipac-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-25 08:41:11.000000 mipac-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-04-25 08:41:27.529852 mipac-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-04-25 08:41:11.000000 mipac-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.529852 mipac-0.4.3/mipac/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-25 08:41:27.529852 mipac-0.4.3/mipac/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.513851 mipac-0.4.3/mipac/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/abstract/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/abstract/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/abstract/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.517851 mipac-0.4.3/mipac/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.517851 mipac-0.4.3/mipac/actions/admins/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/admins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/admins/ad.py
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/admins/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/admins/announcement.py
--rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/admins/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/admins/moderator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/admins/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/admins/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/blocking.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10892 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/favorite.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/federation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/follow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/mute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/my.py
--rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/note.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/actions/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.517851 mipac-0.4.3/mipac/errors/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/errors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/errors/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.521851 mipac-0.4.3/mipac/manager/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.521851 mipac-0.4.3/mipac/manager/admins/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/admins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/admins/ad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/admins/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/admins/announcement.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/admins/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/admins/moderator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/admins/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/admins/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/blocking.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/favorite.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/federation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/follow.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/mute.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/my.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/note.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/page.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/manager/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.525851 mipac-0.4.3/mipac/models/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/ad.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/announcement.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/follow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.525851 mipac-0.4.3/mipac/models/lite/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/lite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/lite/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/lite/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/lite/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/lite/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/lite/note.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/lite/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/mute.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/note.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.529852 mipac-0.4.3/mipac/types/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/achievement.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/ads.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/announcement.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/follow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/mute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/note.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/page.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/types/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.529852 mipac-0.4.3/mipac/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/utils/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-25 08:41:11.000000 mipac-0.4.3/mipac/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:27.513851 mipac-0.4.3/mipac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-04-25 08:41:27.000000 mipac-0.4.3/mipac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-25 08:41:27.000000 mipac-0.4.3/mipac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:41:27.000000 mipac-0.4.3/mipac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-25 08:41:27.000000 mipac-0.4.3/mipac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 08:41:27.000000 mipac-0.4.3/mipac.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-25 08:41:11.000000 mipac-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-25 08:41:11.000000 mipac-0.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-25 08:41:27.529852 mipac-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-25 08:41:11.000000 mipac-0.4.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-25 08:41:11.000000 mipac-0.4.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.727592 mipac-0.4.99/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-18 02:31:31.000000 mipac-0.4.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-18 02:31:31.000000 mipac-0.4.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-18 02:31:40.727592 mipac-0.4.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-06-18 02:31:31.000000 mipac-0.4.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.727592 mipac-0.4.99/mipac/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-18 02:31:40.727592 mipac-0.4.99/mipac/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.715592 mipac-0.4.99/mipac/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/abstract/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/abstract/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/abstract/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.715592 mipac-0.4.99/mipac/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.719592 mipac-0.4.99/mipac/actions/admins/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/admins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/admins/ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/admins/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/admins/announcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/admins/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/admins/moderator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10575 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/admins/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/admins/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/antenna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12007 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/favorite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/federation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/follow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/mute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/my.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.719592 mipac-0.4.99/mipac/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/errors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/errors/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.719592 mipac-0.4.99/mipac/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.719592 mipac-0.4.99/mipac/manager/admins/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/admins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/admins/ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/admins/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/admins/announcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/admins/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/admins/moderator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/admins/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/admins/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/antenna.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/favorite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/federation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/follow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/mute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/my.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.723592 mipac-0.4.99/mipac/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/announcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/antenna.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/follow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.723592 mipac-0.4.99/mipac/models/lite/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/lite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/lite/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/lite/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/lite/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/lite/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/lite/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/lite/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/mute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.727592 mipac-0.4.99/mipac/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/achievement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/ads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/announcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/antenna.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/follow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/mute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.727592 mipac-0.4.99/mipac/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/utils/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/utils/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.715592 mipac-0.4.99/mipac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-18 02:31:40.000000 mipac-0.4.99/mipac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-18 02:31:40.000000 mipac-0.4.99/mipac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:31:40.000000 mipac-0.4.99/mipac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-18 02:31:40.000000 mipac-0.4.99/mipac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-18 02:31:40.000000 mipac-0.4.99/mipac.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-18 02:31:31.000000 mipac-0.4.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 02:31:31.000000 mipac-0.4.99/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-18 02:31:40.727592 mipac-0.4.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-18 02:31:31.000000 mipac-0.4.99/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-18 02:31:31.000000 mipac-0.4.99/versioneer.py
```

### Comparing `mipac-0.4.3/LICENSE` & `mipac-0.4.99/LICENSE`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/PKG-INFO` & `mipac-0.4.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mipac
-Version: 0.4.3
+Version: 0.4.99
 Summary: A Python wrapper for the Misskey API
 Home-page: https://github.com/yupix/mipac
 Author: yupix
 Author-email: yupi0982@outlook.jp
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `mipac-0.4.3/README.md` & `mipac-0.4.99/README.md`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/__init__.py` & `mipac-0.4.99/mipac/__init__.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/actions/admins/ad.py` & `mipac-0.4.99/mipac/actions/admins/ad.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import TYPE_CHECKING, AsyncGenerator, Literal
 
 from mipac.abstract.action import AbstractAction
 from mipac.errors.base import NotSupportVersion, NotSupportVersionText, ParameterError
 from mipac.http import HTTPClient, Route
 from mipac.models.ad import Ad
 from mipac.types.ads import IAd
+from mipac.utils.pagination import Pagination
 
 if TYPE_CHECKING:
     from mipac.client import ClientManager
 
 
 class AdminAdvertisingModelActions(AbstractAction):
     def __init__(self, ad_id: str | None = None, *, session: HTTPClient, client: ClientManager):
@@ -90,35 +91,33 @@
         }
         res: bool = await self._session.request(
             Route('POST', '/api/admin/ad/create'), json=data, auth=True, lower=True
         )
         return res
 
     async def get_list(
-        self, limit: int = 10, since_id: str | None = None, until_id: str | None = None
+        self,
+        limit: int = 10,
+        since_id: str | None = None,
+        until_id: str | None = None,
+        get_all: bool = False,
     ) -> AsyncGenerator[Ad, None]:
         if self._client._config.use_version < 12:
             raise NotSupportVersion(NotSupportVersionText)
 
-        async def request(body) -> list[Ad]:
-            res: list[IAd] = await self._session.request(
-                Route('POST', '/api/admin/ad/list'), lower=True, auth=True, json=body,
-            )
-            return [Ad(ad, client=self._client) for ad in res]
+        if limit > 100:
+            raise ParameterError('limitは100以下である必要があります')
+
+        if get_all:
+            limit = 100
 
         data = {'limit': limit, 'sinceId': since_id, 'untilId': until_id}
-        if all:
-            data['limit'] = 100
-        first_req = await request(data)
-        for ad in first_req:
-            yield ad
-
-        if all and len(first_req) == 100:
-            data['untilId'] = first_req[-1].id
-            while True:
-                res = await request(data)
-                if len(res) <= 100:
-                    for ad in res:
-                        yield ad
-                if len(res) == 0:
-                    break
-                data['untilId'] = res[-1].id
+
+        pagination = Pagination[IAd](self._session, Route('POST', '/api/admin/ad/list'), json=data)
+
+        while True:
+            raw_ads = await pagination.next()
+            for raw_ad in raw_ads:
+                yield Ad(raw_ad, client=self._client)
+
+            if get_all is False or pagination.is_final:
+                break
```

### Comparing `mipac-0.4.3/mipac/actions/admins/admin.py` & `mipac-0.4.99/mipac/actions/admins/admin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, AsyncGenerator
 
 from mipac.abstract.action import AbstractAction
 from mipac.config import config
 from mipac.errors.base import NotSupportVersion, ParameterError
 from mipac.http import HTTPClient, Route
 from mipac.models.admin import IndexStat, ModerationLog, ServerInfo, UserIP
 from mipac.models.meta import AdminMeta
 from mipac.models.user import UserDetailed
 from mipac.types.admin import IIndexStat, IModerationLog, IServerInfo, ITableStats, IUserIP
 from mipac.types.meta import IAdminMeta, IUpdateMetaBody
 from mipac.types.user import IUserDetailed
 from mipac.utils.cache import cache
 from mipac.utils.format import convert_dict_keys_to_camel
+from mipac.utils.pagination import Pagination
 
 if TYPE_CHECKING:
     from mipac.manager.client import ClientManager
 
 
 class AdminActions(AbstractAction):
     def __init__(self, *, session: HTTPClient, client: ClientManager):
@@ -139,27 +140,38 @@
         return bool(
             await self.__session.request(
                 Route('POST', '/api/admin/silence-user'), json={'userId': user_id}, auth=True
             )
         )
 
     async def get_moderation_logs(
-        self, limit: int = 10, since_id: str | None = None, until_id: str | None = None
-    ) -> ModerationLog:
+        self,
+        limit: int = 10,
+        since_id: str | None = None,
+        until_id: str | None = None,
+        get_all: bool = False,
+    ) -> AsyncGenerator[ModerationLog, None]:
         if config.use_version < 12:
             raise NotSupportVersion('ご利用のインスタンスのバージョンではサポートされていない機能です')
 
         if limit > 100:
             raise ParameterError('limit must be less than 100')
 
+        if get_all:
+            limit = 100
+
         body = {'limit': limit, 'sinceId': since_id, 'untilId': until_id}
-        moderation_log_payload: IModerationLog = await self.__session.request(
-            Route('POST', '/api/admin/show-moderation-logs'), json=body, auth=True, lower=True
+        pagination = Pagination[IModerationLog](
+            self.__session, Route('POST', '/api/admin/show-moderation-logs'), json=body
         )
-        return ModerationLog(moderation_log_payload, client=self.__client)
+
+        while True:
+            res_moderation_logs = await pagination.next()
+            for res_moderation_log in res_moderation_logs:
+                yield ModerationLog(res_moderation_log, client=self.__client)
 
     @cache('server_info')
     async def get_server_info(self, **kwargs) -> ServerInfo:
         server_info_payload: IServerInfo = await self.__session.request(
             Route('POST', '/api/admin/server-info'), auth=True, lower=True
         )
         return ServerInfo(server_info_payload)
```

### Comparing `mipac-0.4.3/mipac/actions/admins/announcement.py` & `mipac-0.4.99/mipac/actions/admins/announcement.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import TYPE_CHECKING, AsyncGenerator
 
 from mipac.abstract.action import AbstractAction
 from mipac.errors.base import ParameterError
 from mipac.http import HTTPClient, Route
 from mipac.models.announcement import Announcement, AnnouncementSystem
 from mipac.types.announcement import IAnnouncement, IAnnouncementSystem
+from mipac.utils.pagination import Pagination
 
 if TYPE_CHECKING:
     from mipac.manager.client import ClientManager
 
 
 class AdminAnnouncementClientActions(AbstractAction):
     def __init__(
@@ -65,38 +66,35 @@
             auth=True,
             lower=True,
             remove_none=False,
         )
         return Announcement(created_announcement, client=self.__client)
 
     async def gets(
-        self, limit: int = 10, since_id: str | None = None, until_id: str | None = None,
+        self,
+        limit: int = 10,
+        since_id: str | None = None,
+        until_id: str | None = None,
+        get_all: bool = False,
     ) -> AsyncGenerator[AnnouncementSystem, None]:
         if limit > 100:
             raise ParameterError('limitは100以下である必要があります')
-        if all:
+        if get_all:
             limit = 100
 
-        async def request(req_body) -> list[AnnouncementSystem]:
-            res: list[IAnnouncementSystem] = await self.__session.request(
-                Route('POST', '/api/admin/announcements/list'), auth=True, json=req_body,
-            )
-            return [AnnouncementSystem(announcement, client=self.__client) for announcement in res]
-
         body = {
             'limit': limit,
             'sinceId': since_id,
             'untilId': until_id,
         }
-        first_req = await request(body)
 
-        for announcement in first_req:
-            yield announcement
-        if all and len(first_req) == 100:
-            body['untilId'] = first_req[-1].id
-            while True:
-                res = await request(body)
-                if len(res) <= 100:
-                    for announcement in res:
-                        yield announcement
-                if len(res) < 100:
-                    break
+        pagination = Pagination[IAnnouncementSystem](
+            self.__session, Route('POST', '/api/admin/announcements/list'), json=body
+        )
+
+        while True:
+            res_annonuncement_systems = await pagination.next()
+            for res_announcement_system in res_annonuncement_systems:
+                yield AnnouncementSystem(res_announcement_system, client=self.__client)
+
+            if get_all is False or pagination.is_final:
+                break
```

### Comparing `mipac-0.4.3/mipac/actions/admins/emoji.py` & `mipac-0.4.99/mipac/actions/admins/emoji.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import TYPE_CHECKING, AsyncGenerator
 
 from mipac.abstract.action import AbstractAction
 from mipac.errors.base import NotExistRequiredData, ParameterError
 from mipac.http import Route
 from mipac.models.emoji import CustomEmoji
 from mipac.types.emoji import ICustomEmoji
+from mipac.utils.pagination import Pagination
 from mipac.utils.util import check_multi_arg
 
 if TYPE_CHECKING:
     from mipac.http import HTTPClient
     from mipac.manager.client import ClientManager
 
 
@@ -76,90 +77,84 @@
     async def gets(
         self,
         query: str | None = None,
         limit: int = 10,
         since_id: str | None = None,
         until_id: str | None = None,
         *,
-        all: bool = True
+        get_all: bool = True
     ) -> AsyncGenerator[CustomEmoji, None]:
         if limit > 100:
             raise ParameterError('limitは100以下である必要があります')
-        if all:
+        if get_all:
             limit = 100
 
-        async def request(body) -> list[CustomEmoji]:
-            res: list[ICustomEmoji] = await self.__session.request(
-                Route('POST', '/api/admin/emoji/list'), auth=True, json=body,
-            )
-            return [CustomEmoji(emoji, client=self.__client) for emoji in res]
-
         body = {
             'query': query,
             'limit': limit,
             'sinceId': since_id,
             'untilId': until_id,
         }
-        first_req = await request(body)
 
-        for emoji in first_req:
-            yield emoji
-        if all and len(first_req) == 100:
-            body['untilId'] = first_req[-1].id
-            while True:
-                res = await request(body)
-                if len(res) <= 100:
-                    for emoji in res:
-                        yield emoji
-                if len(res) < 100:
-                    break
+        pagination = Pagination[ICustomEmoji](
+            self.__session, Route('POST', '/api/admin/emoji/list'), json=body
+        )
+
+        while True:
+            res_custom_emojis = await pagination.next()
+            for res_custom_emoji in res_custom_emojis:
+                yield CustomEmoji(res_custom_emoji, client=self.__client)
+
+            if get_all is False or pagination.is_final:
+                break
 
     async def gets_remote(
         self,
         query: str | None = None,
         host: str | None = None,
         limit: int = 10,
         since_id: str | None = None,
         until_id: str | None = None,
         *,
-        all: bool = True
+        get_all: bool = True
     ) -> AsyncGenerator[CustomEmoji, None]:
         if limit > 100:
             raise ParameterError('limitは100以下である必要があります')
-        if all:
+        if get_all:
             limit = 100
 
-        async def request(body) -> list[CustomEmoji]:
-            res: list[ICustomEmoji] = await self.__session.request(
-                Route('POST', '/api/admin/emoji/list-remote'), auth=True, json=body,
-            )
-            return [CustomEmoji(emoji, client=self.__client) for emoji in res]
-
         body = {
             'query': query,
             'host': host,
             'limit': limit,
             'sinceId': since_id,
             'untilId': until_id,
         }
-        first_req = await request(body)
 
-        for note in first_req:
-            yield note
+        pagination = Pagination[ICustomEmoji](
+            self.__session, Route('POST', '/api/admin/emoji/list-remote'), json=body
+        )
 
-        if all and len(first_req) == 100:
-            body['untilId'] = first_req[-1].id
-            while True:
-                res = await request(body)
-                if len(res) <= 100:
-                    for note in res:
-                        yield note
-                if len(res) == 0:
-                    break
-                body['untilId'] = res[-1].id
+        while True:
+            res_custom_emojis = await pagination.next()
+            for res_custom_emoji in res_custom_emojis:
+                yield CustomEmoji(res_custom_emoji, client=self.__client)
+
+            if get_all is False or pagination.is_final:
+                break
+
+    async def set_license_bulk(self, ids: list[str], license: str | None = None) -> bool:
+        body = {'ids': ids, 'license': license}
+        res: bool = await self.__session.request(
+            Route('POST', '/api/admin/emoji/set-license-bulk'),
+            auth=True,
+            json=body,
+            remove_none=False,  # remove_noneをFalseにしないとlisenceが消せなくなる
+        )
+        return res
 
     async def remove(self, emoji_id: str | None = None) -> bool:
         """指定したIdの絵文字を削除します
 
         Parameters
         ----------
         emoji_id : str | None, optional
```

### Comparing `mipac-0.4.3/mipac/actions/admins/moderator.py` & `mipac-0.4.99/mipac/actions/admins/moderator.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/actions/admins/roles.py` & `mipac-0.4.99/mipac/actions/admins/roles.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from mipac.abstract.action import AbstractAction
 from mipac.errors.base import NotSupportVersion, NotSupportVersionText, ParameterError
 from mipac.http import Route
 from mipac.models.roles import Role, RoleUser
 from mipac.types.meta import IPolicies
 from mipac.types.roles import IRole, IRoleUser
+from mipac.utils.pagination import Pagination
 
 if TYPE_CHECKING:
     from mipac.http import HTTPClient
     from mipac.manager.client import ClientManager
 
 
 class AdminRoleModelActions(AbstractAction):
@@ -152,45 +153,43 @@
 
     async def get_users(
         self,
         role_id: str | None = None,
         since_id: str | None = None,
         until_id: str | None = None,
         limit: int = 100,
-        all: bool = False,
+        get_all: bool = False,
     ) -> AsyncGenerator[RoleUser, None]:
+        role_id = self._role_id or role_id
+
         if self._client._config.use_version < 13:
             raise NotSupportVersion(NotSupportVersionText)
-        role_id = self._role_id or role_id
+
         if role_id is None:
             raise ParameterError('role_idは必須です')
 
-        async def request(body) -> list[RoleUser]:
-            res: list[IRoleUser] = await self._session.request(
-                Route('POST', '/api/admin/roles/users'), lower=True, auth=True, json=body,
-            )
-            return [RoleUser(role, client=self._client) for role in res]
+        if limit > 100:
+            raise ParameterError('limitは100以下である必要があります')
+
+        if get_all:
+            limit = 100
+
+        body = {'limit': limit, 'sinceId': since_id, 'untilId': until_id, 'roleId': role_id}
+
+        pagination = Pagination[IRoleUser](
+            self._session, Route('POST', '/api/admin/roles/users'), json=body
+        )
+
+        while True:
+            raw_role_users = await pagination.next()
+            for role_user in raw_role_users:
+                yield RoleUser(role_user, client=self._client)
 
-        data = {'limit': limit, 'sinceId': since_id, 'untilId': until_id, 'roleId': role_id}
-        if all:
-            data['limit'] = 100
-        first_req = await request(data)
-        for user in first_req:
-            yield user
-
-        if all and len(first_req) == 100:
-            data['untilId'] = first_req[-1].id
-            while True:
-                res = await request(data)
-                if len(res) <= 100:
-                    for user in res:
-                        yield user
-                if len(res) == 0:
-                    break
-                data['untilId'] = res[-1].id
+            if get_all is False or pagination.is_final:
+                break
 
 
 class AdminRoleActions(AdminRoleModelActions):
     def __init__(self, role_id: str | None = None, *, session: HTTPClient, client: ClientManager):
         super().__init__(role_id=role_id, session=session, client=client)
 
     async def create(
@@ -203,14 +202,15 @@
         cond_formula: dict[Any, Any] | None = None,
         is_public: bool = False,
         is_moderator: bool = False,
         is_administrator: bool = False,
         as_badge: bool = False,
         can_edit_members_by_moderator: bool = False,
         policies: dict[Any, Any] | None = None,
+        is_explorable: bool = False,
     ) -> Role:
         if self._client._config.use_version >= 13:
             body = {
                 'name': name,
                 'description': description,
                 'color': color,
                 'iconUrl': iconUrl,
@@ -218,14 +218,15 @@
                 'condFormula': cond_formula or {},
                 'isPublic': is_public,
                 'isModerator': is_moderator,
                 'isAdministrator': is_administrator,
                 'asBadge': as_badge,
                 'canEditMembersByModerator': can_edit_members_by_moderator,
                 'policies': policies or {},
+                'isExplorable': is_explorable,
             }
             res: IRole = await self._session.request(
                 Route('POST', '/api/admin/roles/create'),
                 auth=True,
                 json=body,
                 lower=True,
                 remove_none=False,
```

### Comparing `mipac-0.4.3/mipac/actions/admins/user.py` & `mipac-0.4.99/mipac/actions/admins/user.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/actions/blocking.py` & `mipac-0.4.99/mipac/actions/my.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,50 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, AsyncGenerator
+from typing import TYPE_CHECKING
 
 from mipac.abstract.action import AbstractAction
+from mipac.errors.base import NotSupportVersion, NotSupportVersionText
 from mipac.http import HTTPClient, Route
-from mipac.models.user import BlockingUser, UserDetailed
-from mipac.types.user import IBlockingUser, IUserDetailed
+from mipac.models.follow import FollowRequest
+from mipac.types.achievement import IT_ACHIEVEMENT_NAME
+from mipac.types.follow import IFollowRequest
 
 if TYPE_CHECKING:
-    from mipac.client import ClientManager
+    from mipac.manager.client import ClientManager
 
 
-class BlockingActions(AbstractAction):
-    def __init__(self, user_id: str | None = None, *, session: HTTPClient, client: ClientManager):
-        self.__user_id: str | None = user_id
-        self.__session: HTTPClient = session
-        self.__client: ClientManager = client
-
-    async def add(self, user_id: str | None = None) -> UserDetailed:
-        user_id = self.__user_id or user_id
-        res: IUserDetailed = await self.__session.request(
-            Route('POST', '/api/blocking/create'), auth=True, json={'userId': user_id}, lower=True
-        )
-        return UserDetailed(res, client=self.__client)
+class MyActions(AbstractAction):
+    def __init__(self, session: HTTPClient, client: ClientManager):
+        self.__session = session
+        self.__client = client
 
-    async def remove(self, user_id: str | None = None) -> UserDetailed:
-        user_id = self.__user_id or user_id
-        res: IUserDetailed = await self.__session.request(
-            Route('POST', '/api/blocking/delete'), auth=True, json={'userId': user_id}, lower=True
+    async def fetch_follow_requests(self) -> list[FollowRequest]:
+        res: list[IFollowRequest] = await self.__session.request(
+            Route('POST', '/api/following/requests/list'), auth=True, lower=True,
         )
-        return UserDetailed(res, client=self.__client)
+        return [FollowRequest(i, client=self.__client) for i in res]
+
+    async def get_claim_achievement(self, name: IT_ACHIEVEMENT_NAME) -> bool:
+        """指定した名前の実績を解除します
 
-    async def get_list(
-        self,
-        since_id: str | None = None,
-        until_id: str | None = None,
-        limit: int = 100,
-        all: bool = False,
-    ) -> AsyncGenerator[BlockingUser, None]:
-        async def request(body) -> list[BlockingUser]:
-            res: list[IBlockingUser] = await self.__session.request(
-                Route('POST', '/api/blocking/list'), lower=True, auth=True, json=body
-            )
-            return [BlockingUser(user, client=self.__client) for user in res]
-
-        data = {'limit': limit, 'sinceId': since_id, 'untilId': until_id}
-        if all:
-            data['limit'] = 100
-        first_req = await request(data)
-        for user in first_req:
-            yield user
-
-        if all and len(first_req) == 100:
-            data['untilId'] = first_req[-1].id
-            while True:
-                res = await request(data)
-                if len(res) <= 100:
-                    for user in res:
-                        yield user
-                if len(res) == 0:
-                    break
-                data['untilId'] = res[-1].id
+        Parameters
+        ----------
+        name : 実績名
+            解除したい実績の名前
+
+        Returns
+        -------
+        bool
+            成功したか否か
+
+        Raises
+        ------
+        NotSupportVersion
+            実績機能が存在しないサーバーを使用している
+        """
+        if self.__client._config.use_version < 13:
+            raise NotSupportVersion(NotSupportVersionText)
+        res: bool = await self.__session.request(
+            Route('POST', '/api/i/claim-achievement'), auth=True, json={'name': name}, lower=True
+        )
+        return res
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mipac-0.4.3/mipac/actions/channel.py` & `mipac-0.4.99/mipac/actions/channel.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/actions/chart.py` & `mipac-0.4.99/mipac/actions/chart.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/actions/chat.py` & `mipac-0.4.99/mipac/actions/chat.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/actions/client.py` & `mipac-0.4.99/mipac/actions/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from mipac.errors.base import ParameterError
 from mipac.http import HTTPClient, Route
 from mipac.models.announcement import Announcement
 from mipac.models.lite.meta import LiteMeta
 from mipac.models.meta import Meta
 from mipac.types.announcement import IAnnouncement
 from mipac.types.meta import ILiteMeta, IMeta
+from mipac.utils.pagination import Pagination
 
 if TYPE_CHECKING:
     from mipac.manager.client import ClientManager
 
 
 class ClientActions(AbstractAction):
     def __init__(self, *, session: HTTPClient, client: ClientManager) -> None:
@@ -44,39 +45,32 @@
     async def get_announcements(
         self,
         limit: int = 10,
         with_unreads: bool = False,
         since_id: str | None = None,
         until_id: str | None = None,
         *,
-        all: bool = False
+        get_all: bool = False
     ) -> AsyncGenerator[Announcement, None]:
         if limit > 100:
             raise ParameterError('limitは100以下である必要があります')
-        if all:
+        if get_all:
             limit = 100
 
-        async def request(req_body) -> list[Announcement]:
-            res: list[IAnnouncement] = await self.__session.request(
-                Route('POST', '/api/announcements'), auth=True, json=req_body,
-            )
-            return [Announcement(announcement, client=self.__client) for announcement in res]
-
         body = {
             'limit': limit,
             'withUnreads': with_unreads,
             'sinceId': since_id,
             'untilId': until_id,
         }
-        first_req = await request(body)
 
-        for announcement in first_req:
-            yield announcement
-        if all and len(first_req) == 100:
-            body['untilId'] = first_req[-1].id
-            while True:
-                res = await request(body)
-                if len(res) <= 100:
-                    for announcement in res:
-                        yield announcement
-                if len(res) < 100:
-                    break
+        pagination = Pagination[IAnnouncement](
+            self.__session, Route('POST', '/api/announcements'), json=body
+        )
+
+        while True:
+            res_announcements = await pagination.next()
+            for announcement in res_announcements:
+                yield Announcement(announcement, client=self.__client)
+
+            if get_all is False or pagination.is_final:
+                break
```

### Comparing `mipac-0.4.3/mipac/actions/drive.py` & `mipac-0.4.99/mipac/actions/drive.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, AsyncGenerator
 
 from mipac.abstract.action import AbstractAction
 from mipac.errors.base import ParameterError
 from mipac.http import HTTPClient, Route
 from mipac.models.drive import File, Folder
-from mipac.types.drive import IDriveFile
+from mipac.types.drive import FolderPayload, IDriveFile
 from mipac.utils.format import bool_to_string, remove_dict_empty
+from mipac.utils.pagination import Pagination
 from mipac.utils.util import deprecated
 
 if TYPE_CHECKING:
     from mipac.manager.client import ClientManager
 
 __all__ = ('DriveActions', 'FileActions', 'FolderActions')
 
@@ -113,15 +114,16 @@
     async def get_files(
         self,
         limit: int = 10,
         since_id: str | None = None,
         until_id: str | None = None,
         folder_id: str | None = None,
         file_type: str | None = None,
-    ) -> list[File]:
+        get_all: bool = False,
+    ) -> AsyncGenerator[File, None]:
         """
         ファイルを取得します
 
         Parameters
         ----------
         limit : int, default=10
             取得する上限
@@ -133,27 +135,39 @@
             指定すると、そのフォルダーを起点としてファイルを取得します
         file_type : str | None, default=None
             取得したいファイルの拡張子
         """
         if limit > 100:
             raise ParameterError('limit must be less than 100')
 
+        if get_all:
+            limit = 100
+
         folder_id = self._folder_id or folder_id
 
-        data = {
+        body = {
             'limit': limit,
             'sinceId': since_id,
             'untilId': until_id,
             'folderId': folder_id,
             'Type': file_type,
         }
-        res: list[IDriveFile] = await self._session.request(
-            Route('POST', '/api/drive/files'), json=data, auth=True, lower=True
+
+        pagination = Pagination[IDriveFile](
+            self._session, Route('POST', '/api/drive/files'), json=body
         )
-        return [File(i, client=self._client) for i in res]
+
+        while True:
+            res_drive_files = await pagination.next()
+
+            for res_drive_file in res_drive_files:
+                yield File(res_drive_file, client=self._client)
+
+            if get_all is False or pagination.is_final:
+                break
 
     async def upload_file(
         self,
         file: str,
         file_name: str | None = None,
         folder_id: str | None = None,
         comment: str | None = None,
@@ -254,15 +268,16 @@
     async def get_files(
         self,
         limit: int = 10,
         since_id: str | None = None,
         until_id: str | None = None,
         folder_id: str | None = None,
         file_type: str | None = None,
-    ) -> list[File]:
+        get_all: bool = False,
+    ) -> AsyncGenerator[File, None]:
         """
         ファイルを取得します
 
         Parameters
         ----------
         limit : int, default=10
             取得する上限
@@ -274,26 +289,39 @@
             指定すると、そのフォルダーを起点としてファイルを取得します
         file_type : str | None, default=None
             取得したいファイルの拡張子
         """
         if limit > 100:
             raise ParameterError('limit must be less than 100')
 
-        folder_id = folder_id or self._folder_id
-        data = {
+        if get_all:
+            limit = 100
+
+        folder_id = self._folder_id or folder_id
+
+        body = {
             'limit': limit,
             'sinceId': since_id,
             'untilId': until_id,
             'folderId': folder_id,
             'Type': file_type,
         }
-        res: list[IDriveFile] = await self._session.request(
-            Route('POST', '/api/drive/files'), json=data, auth=True, lower=True
+
+        pagination = Pagination[IDriveFile](
+            self._session, Route('POST', '/api/drive/files'), json=body
         )
-        return [File(i, client=self._client) for i in res]
+
+        while True:
+            res_drive_files = await pagination.next()
+
+            for res_drive_file in res_drive_files:
+                yield File(res_drive_file, client=self._client)
+
+            if get_all is False or pagination.is_final:
+                break
 
 
 class FolderActions(ClientFolderActions):
     def __init__(
         self, folder_id: str | None = None, *, session: HTTPClient, client: ClientManager
     ):
         super().__init__(folder_id=folder_id, session=session, client=client)
@@ -306,33 +334,48 @@
 
     async def get_folders(
         self,
         limit: int = 100,
         since_id: str | None = None,
         until_id: str | None = None,
         folder_id: str | None = None,
-    ) -> list[Folder]:
+        get_all: bool = False,
+    ) -> AsyncGenerator[Folder, None]:
         """
         フォルダーの一覧を取得します
 
         Parameters
         ----------
         limit : int, default=10
             取得する上限
         since_id : str | None, default=None
             指定すると、その投稿を投稿を起点としてより新しい投稿を取得します
         until_id : str | None, default=None
             指定すると、その投稿を投稿を起点としてより古い投稿を取得します
         folder_id : str | None, default=None
             指定すると、そのフォルダーを起点としてフォルダーを取得します
+        get_all : bool, default=False
+            Whether to retrieve all folders or not
         """
 
-        data = {
+        if limit > 100:
+            raise ParameterError('limitは100以下である必要があります')
+        if get_all:
+            limit = 100
+
+        body = {
             'limit': limit,
             'sinceId': since_id,
             'untilId': until_id,
             'folderId': folder_id,
         }
-        data = await self._session.request(
-            Route('POST', '/api/drive/folders'), json=data, lower=True, auth=True,
+
+        pagination = Pagination[FolderPayload](
+            self._session, Route('POST', '/api/drive/folders'), json=body
         )
-        return [Folder(i, client=self._client) for i in data]
+
+        while True:
+            res_folders = await pagination.next()
+            for res_folder in res_folders:
+                yield Folder(res_folder, client=self._client)
+            if get_all is False or pagination.is_final:
+                break
```

### Comparing `mipac-0.4.3/mipac/actions/emoji.py` & `mipac-0.4.99/mipac/actions/emoji.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/actions/favorite.py` & `mipac-0.4.99/mipac/actions/favorite.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/actions/federation.py` & `mipac-0.4.99/mipac/actions/federation.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, AsyncGenerator
 
 from mipac.abstract.action import AbstractAction
 from mipac.errors.base import ParameterError
 from mipac.http import HTTPClient, Route
 from mipac.models.instance import FederationInstance
 from mipac.models.user import UserDetailed
 from mipac.types.follow import IFederationFollower, IFederationFollowing
 from mipac.types.instance import IFederationInstance, IFederationInstanceStat
 from mipac.types.user import IUserDetailed
+from mipac.utils.pagination import Pagination
 
 if TYPE_CHECKING:
     from mipac.manager.client import ClientManager
 
 
 class FederationActions(AbstractAction):
     def __init__(self, *, session: HTTPClient, client: ClientManager):
@@ -26,38 +27,79 @@
                 Route('POST', '/api/ap/get'), auth=True, json={'uri': uri}, lower=True
             )
         )
 
     async def show_ap(
         self, host: str, since_id: str | None = None, until_id: str | None = None, limit: int = 10
     ) -> FederationInstance:
+        # TODO: これ本当にuntilId必要なのか確認する
         body = {'host': host, 'sinceId': since_id, 'untilId': until_id, 'limit': limit}
 
         res: FederationInstance = await self.__session.request(
             Route('POST', '/api/ap/show'), auth=True, json=body
         )
         return res
 
     async def get_followers(
-        self, host: str, since_id: str | None = None, until_id: str | None = None, limit: int = 10
+        self,
+        host: str,
+        since_id: str | None = None,
+        until_id: str | None = None,
+        limit: int = 10,
+        get_all: bool = False,
     ):
+
+        if limit > 100:
+            raise ParameterError('limitは100以下である必要があります')
+
+        if get_all:
+            limit = 100
+
         body = {'host': host, 'sinceId': since_id, 'untilId': until_id, 'limit': limit}
-        res: list[IFederationFollower] = await self.__session.request(
-            Route('POST', '/api/federation/followers'), auth=True, json=body, lower=True
+
+        pagination = Pagination[IFederationFollower](
+            self.__session, Route('POST', '/api/federation/followers'), json=body
         )
-        return res
+
+        while True:
+            res_federation_followers: list[IFederationFollower] = await pagination.next()
+            for federation_follower in res_federation_followers:
+                yield federation_follower
+
+            if get_all is False or pagination.is_final:
+                break
 
     async def get_following(
-        self, host: str, since_id: str | None = None, until_id: str | None = None, limit: int = 10
+        self,
+        host: str,
+        since_id: str | None = None,
+        until_id: str | None = None,
+        limit: int = 10,
+        get_all: bool = False,
     ):
+
+        if limit > 100:
+            raise ParameterError('limitは100以下である必要があります')
+
+        if get_all:
+            limit = 100
+
         body = {'host': host, 'sinceId': since_id, 'untilId': until_id, 'limit': limit}
-        res: list[IFederationFollowing] = await self.__session.request(
-            Route('POST', '/api/federation/following'), auth=True, json=body, lower=True
+
+        pagination = Pagination[IFederationFollowing](
+            self.__session, Route('POST', '/api/federation/following'), json=body
         )
-        return res
+
+        while True:
+            res_federation_followings: list[IFederationFollowing] = await pagination.next()
+            for federation_following in res_federation_followings:
+                yield federation_following
+
+            if get_all is False or pagination.is_final:
+                break
 
     async def get_instances(
         self,
         host: str | None = None,
         blocked: bool | None = None,
         not_responding: bool | None = None,
         suspended: bool | None = None,
@@ -105,24 +147,40 @@
                 Route('POST', '/api/federation/update-remote-user'),
                 auth=True,
                 json={'userId': user_id},
             )
         )
 
     async def get_users(
-        self, host: str, since_id: str | None = None, until_id: str | None = None, limit: int = 10
-    ) -> UserDetailed:
+        self,
+        host: str,
+        since_id: str | None = None,
+        until_id: str | None = None,
+        limit: int = 10,
+        get_all: bool = False,
+    ) -> AsyncGenerator[UserDetailed, None]:
         if limit > 100:
             raise ParameterError('limitは100以下である必要があります')
+
+        if get_all:
+            limit = 100
+
         body = {'host': host, 'sinceId': since_id, 'untilId': until_id, 'limit': limit}
 
-        res: IUserDetailed = await self.__session.request(
-            Route('POST', '/api/federation/users'), auth=True, json=body
+        pagination = Pagination[IUserDetailed](
+            self.__session, Route('POST', '/api/federation/users'), json=body
         )
-        return UserDetailed(res, client=self.__client)
+
+        while True:
+            res_users: list[IUserDetailed] = await pagination.next()
+            for user in res_users:
+                yield UserDetailed(user, client=self.__client)
+
+            if get_all is False or pagination.is_final:
+                break
 
     async def get_stats(self, limit: int = 10) -> IFederationInstanceStat:
         if limit > 100:
             raise ParameterError('limitは100以下である必要があります')
         res: IFederationInstanceStat = await self.__session.request(
             Route('POST', '/api/federation/stats'), auth=True, body={'limit': limit}, lower=True
         )
```

### Comparing `mipac-0.4.3/mipac/actions/follow.py` & `mipac-0.4.99/mipac/actions/follow.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/actions/note.py` & `mipac-0.4.99/mipac/actions/note.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from mipac.http import HTTPClient, Route
 from mipac.models.drive import File
 from mipac.models.note import Note, NoteReaction, NoteState, NoteTranslateResult
 from mipac.models.poll import MiPoll, Poll
 from mipac.types.note import ICreatedNote, INote, INoteState, INoteTranslateResult
 from mipac.utils.cache import cache
 from mipac.utils.format import remove_dict_empty
+from mipac.utils.pagination import Pagination
 from mipac.utils.util import check_multi_arg
 
 if TYPE_CHECKING:
     from mipac.client import ClientManager
 
 __all__ = ['NoteActions']
 
@@ -109,47 +110,42 @@
 
     async def get_children(
         self,
         limit: int = 100,
         since_id: str | None = None,
         untilId: str | None = None,
         note_id: str | None = None,
-        all: bool = True,
+        get_all: bool = True,
     ) -> AsyncGenerator[Note, None]:
 
         if limit > 100:
             raise ParameterError('limit は100以下である必要があります')
 
-        async def request(body) -> list[Note]:
-            res: list[INote] = await self._session.request(
-                Route('POST', '/api/notes/children'), lower=True, auth=True, json=body,
-            )
-            return [Note(note, client=self._client) for note in res]
+        if get_all:
+            limit = 100
 
         note_id = note_id or self._note_id
         data = {
             'noteId': note_id,
             'limit': limit,
             'sinceId': since_id,
             'untilId': untilId,
         }
-        first_req = await request(data)
-        for note in first_req:
-            yield note
-
-        if all and len(first_req) == 100:
-            data['untilId'] = first_req[-1].id
-            while True:
-                res = await request(data)
-                if len(res) <= 100:
-                    for note in res:
-                        yield note
-                if len(res) == 0:
-                    break
-                data['untilId'] = res[-1].id
+
+        pagination = Pagination[INote](
+            self._session, Route('POST', '/api/notes/children'), json=data
+        )
+
+        while True:
+            res_notes = await pagination.next()
+            for note in res_notes:
+                yield Note(note, self._client)
+
+            if get_all is False or pagination.is_final:
+                break
 
     async def get_state(self, note_id: str | None = None) -> NoteState:
         note_id = note_id or self._note_id
         data = {'noteId': note_id}
         res: INoteState = await self._session.request(
             Route('POST', '/api/notes/state'), auth=True, json=data
         )
@@ -474,15 +470,16 @@
 
     async def get_replies(
         self,
         since_id: str | None = None,
         until_id: str | None = None,
         limit: int = 10,
         note_id: str | None = None,
-    ) -> list[Note]:
+        get_all: bool = False,
+    ) -> AsyncGenerator[Note, None]:
         """
         ノートに対する返信を取得します
 
         Parameters
         ---------
         since_id : str | None, default=None
             指定すると、その投稿を投稿を起点としてより新しい投稿を取得します
@@ -491,72 +488,71 @@
         limit : int, default=10
             取得する上限
         note_id: str | None, default=None
             返信を取得したいノートのID
 
         Returns
         -------
-        list[Note]
-            返信のリスト
+        AsyncGenerator[Note, None]
+            返信
         """
+
+        if limit > 100:
+            raise ParameterError('limitは100以下である必要があります')
+        if get_all:
+            limit = 100
+
         note_id = note_id or self._note_id
-        res = await self._session.request(
-            Route('POST', '/api/notes/replies'),
-            json={'noteId': note_id, 'sinceId': since_id, 'untilId': until_id, 'limit': limit},
-            auth=True,
-            lower=True,
-        )
-        return [Note(i, client=self._client) for i in res]
+        body = {'noteId': note_id, 'sinceId': since_id, 'untilId': until_id, 'limit': limit}
+
+        pagination = Pagination[INote](self._session, Route('POST', '/api/notes'), json=body)
+
+        while True:
+            res_notes = await pagination.next()
+            for res_note in res_notes:
+                yield Note(res_note, client=self._client)
+
+            if get_all is False or pagination.is_final:
+                break
 
     async def gets(
         self,
         local: bool = False,
         reply: bool = False,
         renote: bool = False,
         with_files: bool = False,
         poll: bool = False,
         limit: int = 100,
         since_id: str | None = None,
         until_id: str | None = None,
         *,
-        all: bool = False,
+        get_all: bool = False,
     ) -> AsyncGenerator[Note, None]:
-
         if limit > 100:
             raise ParameterError('limit は100以下である必要があります')
 
-        async def request(body) -> list[Note]:
-            res: list[INote] = await self._session.request(
-                Route('POST', '/api/notes'), lower=True, auth=True, json=body
-            )
-            return [Note(note, client=self._client) for note in res]
+        if get_all:
+            limit = 100
 
         body = remove_dict_empty(
             {
                 'local': local,
                 'reply': reply,
                 'renote': renote,
                 'withFiles': with_files,
                 'poll': poll,
                 'limit': limit,
                 'sinceId': since_id,
                 'untilId': until_id,
             }
         )
 
-        if all:
-            body['limit'] = 100
-        first_req = await request(body)
-
-        for note in first_req:
-            yield note
-
-        if all and len(first_req) == 100:
-            body['untilId'] = first_req[-1].id
-            while True:
-                res = await request(body)
-                if len(res) <= 100:
-                    for note in res:
-                        yield note
-                if len(res) == 0:
-                    break
-                body['untilId'] = res[-1].id
+        pagination = Pagination[INote](
+            self._session, Route('POST', '/api/notes'), json=body, limit=limit
+        )
+
+        while True:
+            res_notes = await pagination.next()
+            for note in res_notes:
+                yield Note(note, client=self._client)
+            if get_all is False or pagination.is_final:
+                break
```

### Comparing `mipac-0.4.3/mipac/actions/poll.py` & `mipac-0.4.99/mipac/actions/blocking.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,56 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, AsyncGenerator
 
 from mipac.abstract.action import AbstractAction
-from mipac.errors.base import ParameterError
 from mipac.http import HTTPClient, Route
-from mipac.models.note import Note
-from mipac.types.note import INote
+from mipac.models.user import BlockingUser, UserDetailed
+from mipac.types.user import IBlockingUser, IUserDetailed
+from mipac.utils.pagination import Pagination
 
 if TYPE_CHECKING:
-    from mipac.manager.client import ClientManager
+    from mipac.client import ClientManager
 
 
-class PollActions(AbstractAction):
-    def __init__(self, note_id: str | None = None, *, session: HTTPClient, client: ClientManager):
-        self.__note_id: str | None = note_id
+class BlockingActions(AbstractAction):
+    def __init__(self, user_id: str | None = None, *, session: HTTPClient, client: ClientManager):
+        self.__user_id: str | None = user_id
         self.__session: HTTPClient = session
         self.__client: ClientManager = client
 
-    async def vote(self, choice: int, note_id: str | None = None) -> bool:
-        note_id = note_id or self.__note_id
-
-        if note_id is None:
-            raise ParameterError('note_id is required')
+    async def add(self, user_id: str | None = None) -> UserDetailed:
+        user_id = self.__user_id or user_id
+        res: IUserDetailed = await self.__session.request(
+            Route('POST', '/api/blocking/create'), auth=True, json={'userId': user_id}, lower=True
+        )
+        return UserDetailed(res, client=self.__client)
 
-        data = {'noteId': note_id, 'choice': choice}
-        res: bool = await self.__session.request(
-            Route('POST', '/api/notes/polls/vote'), auth=True, json=data
+    async def remove(self, user_id: str | None = None) -> UserDetailed:
+        user_id = self.__user_id or user_id
+        res: IUserDetailed = await self.__session.request(
+            Route('POST', '/api/blocking/delete'), auth=True, json={'userId': user_id}, lower=True
         )
-        return res
+        return UserDetailed(res, client=self.__client)
 
-    async def recommendation(self, limit: int = 100, offset: int = 0, all: bool = True):
+    async def get_list(
+        self,
+        since_id: str | None = None,
+        until_id: str | None = None,
+        limit: int = 100,
+        get_all: bool = False,
+    ) -> AsyncGenerator[BlockingUser, None]:
+        if get_all:
+            limit = 100
 
-        if limit > 100:
-            raise ParameterError('limit must be less than 100')
+        data = {'limit': limit, 'sinceId': since_id, 'untilId': until_id}
 
-        if all:
-            limit = 100
+        pagination = Pagination[IBlockingUser](
+            self.__session, Route('POST', '/api/blocking/list'), json=data
+        )
 
-        async def request(body) -> list[Note]:
-            res: list[INote] = await self.__session.request(
-                Route('POST', '/api/notes/polls/recommendation'), lower=True, auth=True, json=body,
-            )
-            return [Note(note, client=self.__client) for note in res]
-
-        data = {'limit': limit, 'offset': offset}
-        first_res: list[Note] = await request(data)
-        for note in first_res:
-            yield note
-        offset = limit
-        count = 1
-        if all and len(first_res) == limit:
-            data['offset'] = limit * count
-            while True:
-                res = await request(data)
-                if len(res) <= limit:
-                    for note in res:
-                        yield note
-                if len(res) == 0 or len(res) < limit:
-                    break
-                data['offset'] = limit * count
-                count = count + 1
+        while True:
+            res_users = await pagination.next()
+            for user in res_users:
+                yield BlockingUser(user, client=self.__client)
+            if get_all is False or pagination.is_final:
+                break
```

### Comparing `mipac-0.4.3/mipac/actions/reaction.py` & `mipac-0.4.99/mipac/actions/reaction.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/actions/user.py` & `mipac-0.4.99/mipac/actions/user.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, AsyncGenerator, Literal, Optional
 
 from mipac.config import config
 from mipac.errors.base import NotExistRequiredData, NotSupportVersion, ParameterError
 from mipac.http import HTTPClient, Route
+from mipac.models.note import Note
 from mipac.models.user import Achievement, LiteUser, UserDetailed
+from mipac.types.note import INote
 from mipac.utils.cache import cache
 from mipac.utils.format import remove_dict_empty
+from mipac.utils.pagination import Pagination
 from mipac.utils.util import check_multi_arg
 
 if TYPE_CHECKING:
     from mipac.manager.client import ClientManager
-    from mipac.models.note import Note
 
 __all__ = ['UserActions']
 
 
 class UserActions:
     def __init__(
         self, session: HTTPClient, client: ClientManager, user: Optional[LiteUser] = None,
@@ -112,18 +114,19 @@
         until_id: str | None = None,
         since_date: int = 0,
         until_date: int = 0,
         include_my_renotes: bool = True,
         with_files: bool = False,
         file_type: Optional[list[str]] = None,
         exclude_nsfw: bool = True,
-    ) -> list[Note]:
+        get_all: bool = False,
+    ) -> AsyncGenerator[Note, None]:
 
-        if check_multi_arg(user_id, self.__user):
-            raise ParameterError('user_idがありません')
+        if check_multi_arg(user_id, self.__user) is False:
+            raise ParameterError('user_idがありません', user_id, self.__user)
 
         user_id = user_id or self.__user and self.__user.id
         data = {
             'userId': user_id,
             'includeReplies': include_replies,
             'limit': limit,
             'sinceId': since_id,
@@ -131,18 +134,29 @@
             'sinceDate': since_date,
             'untilDate': until_date,
             'includeMyRenotes': include_my_renotes,
             'withFiles': with_files,
             'fileType': file_type,
             'excludeNsfw': exclude_nsfw,
         }
-        res = await self.__session.request(
-            Route('POST', '/api/users/notes'), json=data, auth=True, lower=True
+
+        if get_all:
+            data['limit'] = 100
+            limit = 100
+
+        pagination = Pagination[INote](
+            self.__session, Route('POST', '/api/users/notes'), json=data, limit=limit
         )
-        return [Note(i, client=self.__client) for i in res]
+
+        while True:
+            res_notes = await pagination.next()
+            for note in res_notes:
+                yield Note(note, client=self.__client)
+            if get_all is False or pagination.is_final:
+                break
 
     def get_mention(self, user: Optional[LiteUser] = None) -> str:
         """
         Get mention name of user.
 
         Parameters
         ----------
@@ -165,15 +179,15 @@
         self,
         query: str,
         limit: int = 100,
         offset: int = 0,
         origin: Literal['local', 'remote', 'combined'] = 'combined',
         detail: bool = True,
         *,
-        all: bool = False,
+        get_all: bool = False,
     ) -> AsyncGenerator[UserDetailed | LiteUser, None]:
         """
         Search users by keyword.
 
         Parameters
         ----------
         query : str
@@ -182,59 +196,43 @@
             The maximum number of users to return.
         offset : int, default=0
             The number of users to skip.
         origin : Literal['local', 'remote', 'combined'], default='combined'
             The origin of users to search.
         detail : bool, default=True
             Whether to return detailed user information.
-        all : bool, default=False
+        get_all : bool, default=False
             Whether to return all users.
 
         Returns
         -------
         AsyncGenerator[UserDetailed | LiteUser, None]
             A AsyncGenerator of users.
         """
 
         if limit > 100:
             raise ParameterError('limit は100以下である必要があります')
 
-        async def request(body) -> list[UserDetailed | LiteUser]:
-            res = await self.__session.request(
-                Route('POST', '/api/users/search'), lower=True, auth=True, json=body,
-            )
-            return [
-                UserDetailed(user, client=self.__client)
-                if detail
-                else LiteUser(user, client=self.__client)
-                for user in res
-            ]
+        if get_all:
+            limit = 100
 
         body = remove_dict_empty(
             {'query': query, 'limit': limit, 'offset': offset, 'origin': origin, 'detail': detail}
         )
 
-        if all:
-            body['limit'] = 100
-        first_req = await request(body)
-
-        for user in first_req:
-            yield user
-
-        if all and len(first_req) == 100:
-            times = 1
-            while True:
-                body['offset'] = times * 100
-                res = await request(body)
-                if len(res) <= 100:
-                    for user in res:
-                        yield user
-                if len(res) == 0:
-                    break
-                times += 1
+        pagination = Pagination[UserDetailed | LiteUser](
+            self.__session, Route('POST', '/api/users/search'), json=body, pagination_type='count'
+        )
+
+        while True:
+            res_users = await pagination.next()
+            for user in res_users:
+                yield UserDetailed(user, client=self.__client) if detail else LiteUser(user, client=self.__client)  # type: ignore
+            if get_all is False or pagination.is_final:
+                break
 
     async def search_by_username_and_host(
         self, username: str, host: str, limit: int = 100, detail: bool = True,
     ) -> list[UserDetailed | LiteUser]:
         """
         Search users by username and host.
```

### Comparing `mipac-0.4.3/mipac/client.py` & `mipac-0.4.99/mipac/client.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/config.py` & `mipac-0.4.99/mipac/config.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/errors/base.py` & `mipac-0.4.99/mipac/errors/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.message: str | None = None
         if isinstance(data, dict):
             error = data.get('error', {})
             if isinstance(error, dict):
                 self.code: str | None = error.get('code', '')
                 self.id: str | None = error.get('id')
                 self.message: str | None = error.get('message', '')
-        super().__init__(self.message or self.raw)
+        super().__init__(f'{self.message}\nRaw error: {self.raw} ' if self.message else self.raw)
 
     def raise_error(self):
         if not self.code:
             raise self
         if value := getattr(
             import_module('mipac.errors.errors'),
             ''.join([i.capitalize() for i in self.code.split('_')]) + 'Error',
```

### Comparing `mipac-0.4.3/mipac/errors/errors.py` & `mipac-0.4.99/mipac/errors/errors.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/file.py` & `mipac-0.4.99/mipac/file.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/http.py` & `mipac-0.4.99/mipac/http.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/manager/admins/ad.py` & `mipac-0.4.99/mipac/manager/admins/ad.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/manager/admins/admin.py` & `mipac-0.4.99/mipac/manager/admins/admin.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/manager/admins/announcement.py` & `mipac-0.4.99/mipac/manager/admins/announcement.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/manager/admins/emoji.py` & `mipac-0.4.99/mipac/manager/admins/emoji.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/manager/admins/moderator.py` & `mipac-0.4.99/mipac/manager/admins/moderator.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/manager/admins/roles.py` & `mipac-0.4.99/mipac/manager/admins/roles.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/manager/admins/user.py` & `mipac-0.4.99/mipac/manager/admins/user.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/manager/blocking.py` & `mipac-0.4.99/mipac/manager/blocking.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/manager/channel.py` & `mipac-0.4.99/mipac/manager/channel.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/manager/chart.py` & `mipac-0.4.99/mipac/manager/chart.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/manager/chat.py` & `mipac-0.4.99/mipac/manager/chat.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/manager/client.py` & `mipac-0.4.99/mipac/manager/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from mipac.actions.client import ClientActions
 from mipac.http import HTTPClient
 from mipac.manager.admins.admin import AdminManager
+from mipac.manager.antenna import AntennaManager
 from mipac.manager.channel import ChannelManager
 from mipac.manager.chart import ChartManager
 from mipac.manager.chat import ChatManager
 from mipac.manager.drive import DriveManager
 from mipac.manager.emoji import EmojiManager
 from mipac.manager.follow import FollowManager, FollowRequestManager
 from mipac.manager.my import MyManager
@@ -38,14 +39,15 @@
         self.follow: FollowManager = FollowManager(
             session=session, client=self,
         )
         self.follow_request: FollowRequestManager = FollowRequestManager(
             session=session, client=self,
         )
         self.emoji: EmojiManager = EmojiManager(session=session, client=self)
+        self.antenna: AntennaManager = AntennaManager(session=session, client=self)
         self._config: Config = config
 
     @property
     def action(self) -> ClientActions:
         return ClientActions(session=self.__session, client=self)
 
     def _create_user_instance(self, user: LiteUser) -> UserManager:
```

### Comparing `mipac-0.4.3/mipac/manager/drive.py` & `mipac-0.4.99/mipac/manager/drive.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/manager/emoji.py` & `mipac-0.4.99/mipac/manager/emoji.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/manager/favorite.py` & `mipac-0.4.99/mipac/manager/favorite.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/manager/federation.py` & `mipac-0.4.99/mipac/manager/federation.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/manager/follow.py` & `mipac-0.4.99/mipac/manager/follow.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/manager/mute.py` & `mipac-0.4.99/mipac/manager/mute.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/manager/my.py` & `mipac-0.4.99/mipac/manager/my.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/manager/page.py` & `mipac-0.4.99/mipac/manager/page.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/manager/poll.py` & `mipac-0.4.99/mipac/manager/poll.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/manager/reaction.py` & `mipac-0.4.99/mipac/manager/reaction.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/manager/user.py` & `mipac-0.4.99/mipac/manager/user.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/ad.py` & `mipac-0.4.99/mipac/models/ad.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/admin.py` & `mipac-0.4.99/mipac/models/admin.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/announcement.py` & `mipac-0.4.99/mipac/models/announcement.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/channel.py` & `mipac-0.4.99/mipac/models/channel.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/chart.py` & `mipac-0.4.99/mipac/models/chart.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/chat.py` & `mipac-0.4.99/mipac/models/chat.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/drive.py` & `mipac-0.4.99/mipac/models/drive.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/emoji.py` & `mipac-0.4.99/mipac/models/emoji.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/follow.py` & `mipac-0.4.99/mipac/models/follow.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/instance.py` & `mipac-0.4.99/mipac/models/instance.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/lite/channel.py` & `mipac-0.4.99/mipac/models/lite/channel.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/lite/emoji.py` & `mipac-0.4.99/mipac/models/lite/emoji.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/lite/instance.py` & `mipac-0.4.99/mipac/models/lite/instance.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/lite/meta.py` & `mipac-0.4.99/mipac/models/lite/meta.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/lite/note.py` & `mipac-0.4.99/mipac/models/lite/note.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/lite/user.py` & `mipac-0.4.99/mipac/models/lite/user.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/meta.py` & `mipac-0.4.99/mipac/models/meta.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/mute.py` & `mipac-0.4.99/mipac/models/mute.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/note.py` & `mipac-0.4.99/mipac/models/note.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/notification.py` & `mipac-0.4.99/mipac/models/notification.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/poll.py` & `mipac-0.4.99/mipac/models/poll.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/reaction.py` & `mipac-0.4.99/mipac/models/reaction.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/roles.py` & `mipac-0.4.99/mipac/models/roles.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/models/user.py` & `mipac-0.4.99/mipac/models/user.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/types/achievement.py` & `mipac-0.4.99/mipac/types/achievement.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     'followers500',
     'followers1000',
     'collectAchievements30',
     'viewAchievements3min',
     'iLoveMisskey',
     'foundTreasure',
     'client30min',
+    'client60min',
     'noteDeletedWithin1min',
     'postedAtLateNight',
     'postedAt0min0sec',
     'selfQuote',
     'htl20npm',
     'viewInstanceChart',
     'outputHelloWorldOnScratchpad',
```

### Comparing `mipac-0.4.3/mipac/types/admin.py` & `mipac-0.4.99/mipac/types/admin.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/types/channel.py` & `mipac-0.4.99/mipac/types/channel.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/types/chart.py` & `mipac-0.4.99/mipac/types/chart.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/types/chat.py` & `mipac-0.4.99/mipac/types/chat.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/types/drive.py` & `mipac-0.4.99/mipac/types/drive.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/types/emoji.py` & `mipac-0.4.99/mipac/types/emoji.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/types/endpoints.py` & `mipac-0.4.99/mipac/types/endpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,16 +348,15 @@
     '/api/users/groups/joined',
     '/api/users/groups/owned',
     '/api/users/groups/pull',
     '/api/users/groups/show',
     '/api/users/groups/transfer',
     '/api/users/groups/update',
     '/api/version',
-    '/api/admin/queue/promote',
     '/api/channels/favorite',
     '/api/channels/unfavorite',
     '/api/channels/my-favorites',
     '/api/channels/search',
-    '/api/emoji',
     '/api/roles/notes',
     '/api/users/update-memo',
+    '/api/admin/emoji/set-license-bulk'
 ]
```

### Comparing `mipac-0.4.3/mipac/types/instance.py` & `mipac-0.4.99/mipac/types/instance.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/types/meta.py` & `mipac-0.4.99/mipac/types/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,7 +254,8 @@
     object_storage_port: int | None
     object_storage_access_key: str | None
     object_storage_secret_key: str | None
     object_storage_use_s_s_l: bool
     object_storage_use_proxy: bool
     object_storage_set_public_read: bool
     object_storage_s3_force_path_style: bool
+    server_rules: NotRequired[list[str]]  # v13.11.3以降のバージョンから追加。その場合は使わないとエラー出るかも
```

### Comparing `mipac-0.4.3/mipac/types/note.py` & `mipac-0.4.99/mipac/types/note.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/types/notification.py` & `mipac-0.4.99/mipac/types/notification.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/types/page.py` & `mipac-0.4.99/mipac/types/page.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/types/roles.py` & `mipac-0.4.99/mipac/types/roles.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/types/user.py` & `mipac-0.4.99/mipac/types/user.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/util.py` & `mipac-0.4.99/mipac/util.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/utils/auth.py` & `mipac-0.4.99/mipac/utils/auth.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/utils/cache.py` & `mipac-0.4.99/mipac/utils/cache.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/utils/format.py` & `mipac-0.4.99/mipac/utils/format.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/utils/log.py` & `mipac-0.4.99/mipac/utils/log.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac/utils/util.py` & `mipac-0.4.99/mipac/utils/util.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/mipac.egg-info/PKG-INFO` & `mipac-0.4.99/mipac.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mipac
-Version: 0.4.3
+Version: 0.4.99
 Summary: A Python wrapper for the Misskey API
 Home-page: https://github.com/yupix/mipac
 Author: yupix
 Author-email: yupi0982@outlook.jp
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `mipac-0.4.3/mipac.egg-info/SOURCES.txt` & `mipac-0.4.99/mipac.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 mipac.egg-info/requires.txt
 mipac.egg-info/top_level.txt
 mipac/abstract/__init__.py
 mipac/abstract/action.py
 mipac/abstract/manager.py
 mipac/abstract/model.py
 mipac/actions/__init__.py
+mipac/actions/antenna.py
 mipac/actions/blocking.py
 mipac/actions/channel.py
 mipac/actions/chart.py
 mipac/actions/chat.py
 mipac/actions/client.py
 mipac/actions/drive.py
 mipac/actions/emoji.py
@@ -47,14 +48,15 @@
 mipac/actions/admins/moderator.py
 mipac/actions/admins/roles.py
 mipac/actions/admins/user.py
 mipac/errors/__init__.py
 mipac/errors/base.py
 mipac/errors/errors.py
 mipac/manager/__init__.py
+mipac/manager/antenna.py
 mipac/manager/blocking.py
 mipac/manager/channel.py
 mipac/manager/chart.py
 mipac/manager/chat.py
 mipac/manager/client.py
 mipac/manager/drive.py
 mipac/manager/emoji.py
@@ -76,14 +78,15 @@
 mipac/manager/admins/moderator.py
 mipac/manager/admins/roles.py
 mipac/manager/admins/user.py
 mipac/models/__init__.py
 mipac/models/ad.py
 mipac/models/admin.py
 mipac/models/announcement.py
+mipac/models/antenna.py
 mipac/models/channel.py
 mipac/models/chart.py
 mipac/models/chat.py
 mipac/models/drive.py
 mipac/models/emoji.py
 mipac/models/follow.py
 mipac/models/instance.py
@@ -103,14 +106,15 @@
 mipac/models/lite/note.py
 mipac/models/lite/user.py
 mipac/types/__init__.py
 mipac/types/achievement.py
 mipac/types/admin.py
 mipac/types/ads.py
 mipac/types/announcement.py
+mipac/types/antenna.py
 mipac/types/channel.py
 mipac/types/chart.py
 mipac/types/chat.py
 mipac/types/drive.py
 mipac/types/emoji.py
 mipac/types/endpoints.py
 mipac/types/follow.py
@@ -125,8 +129,9 @@
 mipac/types/roles.py
 mipac/types/user.py
 mipac/utils/__init__.py
 mipac/utils/auth.py
 mipac/utils/cache.py
 mipac/utils/format.py
 mipac/utils/log.py
+mipac/utils/pagination.py
 mipac/utils/util.py
```

### Comparing `mipac-0.4.3/setup.py` & `mipac-0.4.99/setup.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.3/versioneer.py` & `mipac-0.4.99/versioneer.py`

 * *Files identical despite different names*

