# Comparing `tmp/dimples-0.1.8.tar.gz` & `tmp/dimples-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dimples-0.1.8.tar", last modified: Mon Jun 12 15:42:23 2023, max compression
+gzip compressed data, was "dist/dimples-0.2.0.tar", last modified: Sun Jun 18 14:42:05 2023, max compression
```

## Comparing `dimples-0.1.8.tar` & `dimples-0.2.0.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2023-06-12 15:42:23.000000 dimples-0.1.8/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-0.1.8/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/
--rw-r--r--   0 moky       (501) staff       (20)     7204 2023-06-10 12:29:39.000000 dimples-0.1.8/dimples/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/client/
--rw-r--r--   0 moky       (501) staff       (20)     1997 2023-06-03 11:38:39.000000 dimples-0.1.8/dimples/client/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/client/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     2191 2023-06-09 16:37:34.000000 dimples-0.1.8/dimples/client/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4011 2023-06-02 18:30:20.000000 dimples-0.1.8/dimples/client/cpu/grp_expel.py
--rw-r--r--   0 moky       (501) staff       (20)     4116 2023-06-02 18:31:07.000000 dimples-0.1.8/dimples/client/cpu/grp_invite.py
--rw-r--r--   0 moky       (501) staff       (20)     3554 2023-02-23 11:18:06.000000 dimples-0.1.8/dimples/client/cpu/grp_query.py
--rw-r--r--   0 moky       (501) staff       (20)     3558 2023-06-02 18:31:36.000000 dimples-0.1.8/dimples/client/cpu/grp_quit.py
--rw-r--r--   0 moky       (501) staff       (20)     6498 2023-06-02 18:32:15.000000 dimples-0.1.8/dimples/client/cpu/grp_reset.py
--rw-r--r--   0 moky       (501) staff       (20)     5150 2023-02-23 14:17:47.000000 dimples-0.1.8/dimples/client/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     2948 2023-01-31 05:28:07.000000 dimples-0.1.8/dimples/client/cpu/history.py
--rw-r--r--   0 moky       (501) staff       (20)     1869 2023-01-31 05:28:07.000000 dimples-0.1.8/dimples/client/cpu/login.py
--rw-r--r--   0 moky       (501) staff       (20)     1847 2023-01-31 05:28:07.000000 dimples-0.1.8/dimples/client/cpu/receipt.py
--rw-r--r--   0 moky       (501) staff       (20)     1895 2023-06-09 16:41:36.000000 dimples-0.1.8/dimples/client/cpu/text.py
--rw-r--r--   0 moky       (501) staff       (20)    16324 2023-06-02 17:03:56.000000 dimples-0.1.8/dimples/client/group.py
--rw-r--r--   0 moky       (501) staff       (20)     9951 2023-06-12 14:16:50.000000 dimples-0.1.8/dimples/client/messenger.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/client/network/
--rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-0.1.8/dimples/client/network/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6258 2023-02-23 14:14:03.000000 dimples-0.1.8/dimples/client/network/session.py
--rw-r--r--   0 moky       (501) staff       (20)     8302 2023-06-03 11:39:42.000000 dimples-0.1.8/dimples/client/network/state.py
--rw-r--r--   0 moky       (501) staff       (20)     9531 2023-01-31 05:28:07.000000 dimples-0.1.8/dimples/client/network/transition.py
--rw-r--r--   0 moky       (501) staff       (20)     6619 2023-06-12 13:22:46.000000 dimples-0.1.8/dimples/client/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     7190 2023-06-09 16:42:29.000000 dimples-0.1.8/dimples/client/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5521 2023-02-23 14:13:41.000000 dimples-0.1.8/dimples/client/terminal.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/common/
--rw-r--r--   0 moky       (501) staff       (20)     2209 2023-06-06 13:30:28.000000 dimples-0.1.8/dimples/common/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4322 2023-06-02 08:44:29.000000 dimples-0.1.8/dimples/common/ans.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/common/dbi/
--rw-r--r--   0 moky       (501) staff       (20)     2324 2023-06-09 14:20:27.000000 dimples-0.1.8/dimples/common/dbi/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6396 2023-06-02 10:33:41.000000 dimples-0.1.8/dimples/common/dbi/account.py
--rw-r--r--   0 moky       (501) staff       (20)     2465 2023-06-02 07:39:55.000000 dimples-0.1.8/dimples/common/dbi/message.py
--rw-r--r--   0 moky       (501) staff       (20)     7877 2023-06-09 15:01:59.000000 dimples-0.1.8/dimples/common/dbi/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6739 2023-06-02 09:05:19.000000 dimples-0.1.8/dimples/common/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     7827 2023-06-12 14:51:01.000000 dimples-0.1.8/dimples/common/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     7710 2023-06-12 13:20:42.000000 dimples-0.1.8/dimples/common/packer.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/common/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     2536 2023-02-23 09:20:27.000000 dimples-0.1.8/dimples/common/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3321 2023-06-09 16:01:10.000000 dimples-0.1.8/dimples/common/protocol/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     5004 2022-12-23 07:24:37.000000 dimples-0.1.8/dimples/common/protocol/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4523 2023-06-02 08:11:42.000000 dimples-0.1.8/dimples/common/protocol/login.py
--rw-r--r--   0 moky       (501) staff       (20)     6085 2023-06-02 08:40:15.000000 dimples-0.1.8/dimples/common/protocol/receipt.py
--rw-r--r--   0 moky       (501) staff       (20)     2521 2023-06-02 08:42:45.000000 dimples-0.1.8/dimples/common/protocol/report.py
--rw-r--r--   0 moky       (501) staff       (20)     4486 2023-06-04 16:41:38.000000 dimples-0.1.8/dimples/common/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6211 2023-06-03 12:24:47.000000 dimples-0.1.8/dimples/config.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/conn/
--rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-0.1.8/dimples/conn/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10335 2023-06-07 13:23:28.000000 dimples-0.1.8/dimples/conn/gate.py
--rw-r--r--   0 moky       (501) staff       (20)     9892 2023-01-31 05:28:07.000000 dimples-0.1.8/dimples/conn/gatekeeper.py
--rw-r--r--   0 moky       (501) staff       (20)    10305 2023-01-14 13:25:42.000000 dimples-0.1.8/dimples/conn/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     7851 2023-02-23 09:10:59.000000 dimples-0.1.8/dimples/conn/mtp.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/conn/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/conn/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8711 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/conn/protocol/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     8254 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/conn/protocol/ws.py
--rw-r--r--   0 moky       (501) staff       (20)     5411 2023-02-23 09:10:59.000000 dimples-0.1.8/dimples/conn/queue.py
--rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-0.1.8/dimples/conn/seeker.py
--rw-r--r--   0 moky       (501) staff       (20)     5726 2023-06-02 09:57:33.000000 dimples-0.1.8/dimples/conn/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6991 2023-01-14 12:47:37.000000 dimples-0.1.8/dimples/conn/ws.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/database/
--rw-r--r--   0 moky       (501) staff       (20)     2560 2023-06-04 16:46:57.000000 dimples-0.1.8/dimples/database/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7000 2023-06-02 12:26:57.000000 dimples-0.1.8/dimples/database/account.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/database/dos/
--rw-r--r--   0 moky       (501) staff       (20)     1808 2023-06-05 05:13:02.000000 dimples-0.1.8/dimples/database/dos/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4071 2022-12-22 17:59:17.000000 dimples-0.1.8/dimples/database/dos/base.py
--rw-r--r--   0 moky       (501) staff       (20)     3769 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/database/dos/document.py
--rw-r--r--   0 moky       (501) staff       (20)     4232 2023-06-02 10:30:44.000000 dimples-0.1.8/dimples/database/dos/group.py
--rw-r--r--   0 moky       (501) staff       (20)     3141 2023-06-02 11:02:33.000000 dimples-0.1.8/dimples/database/dos/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2680 2022-12-22 17:58:13.000000 dimples-0.1.8/dimples/database/dos/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5630 2023-06-02 11:04:20.000000 dimples-0.1.8/dimples/database/dos/private.py
--rw-r--r--   0 moky       (501) staff       (20)     8033 2023-06-09 14:40:24.000000 dimples-0.1.8/dimples/database/dos/station.py
--rw-r--r--   0 moky       (501) staff       (20)     5625 2023-06-02 11:01:02.000000 dimples-0.1.8/dimples/database/dos/user.py
--rw-r--r--   0 moky       (501) staff       (20)     3097 2022-12-13 10:56:52.000000 dimples-0.1.8/dimples/database/message.py
--rw-r--r--   0 moky       (501) staff       (20)     4229 2023-06-04 17:05:32.000000 dimples-0.1.8/dimples/database/session.py
--rw-r--r--   0 moky       (501) staff       (20)     2972 2023-01-31 05:28:07.000000 dimples-0.1.8/dimples/database/t_cipherkey.py
--rw-r--r--   0 moky       (501) staff       (20)     3710 2023-06-09 14:19:20.000000 dimples-0.1.8/dimples/database/t_document.py
--rw-r--r--   0 moky       (501) staff       (20)     7715 2023-06-05 05:41:56.000000 dimples-0.1.8/dimples/database/t_group.py
--rw-r--r--   0 moky       (501) staff       (20)     3718 2023-06-09 14:19:56.000000 dimples-0.1.8/dimples/database/t_login.py
--rw-r--r--   0 moky       (501) staff       (20)     5144 2022-12-22 18:03:37.000000 dimples-0.1.8/dimples/database/t_message.py
--rw-r--r--   0 moky       (501) staff       (20)     3513 2023-06-05 05:36:10.000000 dimples-0.1.8/dimples/database/t_meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5589 2023-06-05 05:38:08.000000 dimples-0.1.8/dimples/database/t_private.py
--rw-r--r--   0 moky       (501) staff       (20)     6647 2023-06-05 05:31:39.000000 dimples-0.1.8/dimples/database/t_station.py
--rw-r--r--   0 moky       (501) staff       (20)     6455 2023-06-05 05:39:18.000000 dimples-0.1.8/dimples/database/t_user.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/edge/
--rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/edge/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    13567 2023-06-12 14:07:59.000000 dimples-0.1.8/dimples/edge/octopus.py
--rw-r--r--   0 moky       (501) staff       (20)     5594 2023-06-05 05:51:39.000000 dimples-0.1.8/dimples/edge/shared.py
--rw-r--r--   0 moky       (501) staff       (20)     2726 2023-06-04 10:23:09.000000 dimples-0.1.8/dimples/edge/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/register/
--rw-r--r--   0 moky       (501) staff       (20)     1441 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/register/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     9516 2023-06-02 10:01:29.000000 dimples-0.1.8/dimples/register/generate.py
--rw-r--r--   0 moky       (501) staff       (20)     7045 2023-06-02 10:02:10.000000 dimples-0.1.8/dimples/register/modify.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3880 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/register/run.py
--rw-r--r--   0 moky       (501) staff       (20)     1971 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/register/shared.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/server/
--rw-r--r--   0 moky       (501) staff       (20)     2561 2023-06-07 12:19:50.000000 dimples-0.1.8/dimples/server/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/server/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     1855 2023-02-23 09:37:38.000000 dimples-0.1.8/dimples/server/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2640 2023-02-23 10:54:44.000000 dimples-0.1.8/dimples/server/cpu/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     4781 2023-06-03 12:02:30.000000 dimples-0.1.8/dimples/server/cpu/document.py
--rw-r--r--   0 moky       (501) staff       (20)     3464 2023-06-12 12:55:43.000000 dimples-0.1.8/dimples/server/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     3853 2023-06-03 12:02:46.000000 dimples-0.1.8/dimples/server/cpu/login.py
--rw-r--r--   0 moky       (501) staff       (20)     1847 2023-01-31 05:28:07.000000 dimples-0.1.8/dimples/server/cpu/receipt.py
--rw-r--r--   0 moky       (501) staff       (20)     3089 2023-01-31 05:28:07.000000 dimples-0.1.8/dimples/server/cpu/report.py
--rw-r--r--   0 moky       (501) staff       (20)    13580 2023-06-12 12:40:57.000000 dimples-0.1.8/dimples/server/dispatcher.py
--rw-r--r--   0 moky       (501) staff       (20)    14053 2023-06-12 15:03:48.000000 dimples-0.1.8/dimples/server/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     6659 2023-06-09 08:36:13.000000 dimples-0.1.8/dimples/server/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     5791 2023-02-23 11:39:56.000000 dimples-0.1.8/dimples/server/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     6443 2023-06-09 13:36:28.000000 dimples-0.1.8/dimples/server/push_info.py
--rw-r--r--   0 moky       (501) staff       (20)     6719 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/server/push_service.py
--rw-r--r--   0 moky       (501) staff       (20)     5877 2023-06-07 13:18:30.000000 dimples-0.1.8/dimples/server/pusher.py
--rw-r--r--   0 moky       (501) staff       (20)     7986 2023-01-14 12:19:38.000000 dimples-0.1.8/dimples/server/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/server/session_center.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/station/
--rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-0.1.8/dimples/station/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4624 2023-06-07 12:21:10.000000 dimples-0.1.8/dimples/station/handler.py
--rw-r--r--   0 moky       (501) staff       (20)     7087 2023-06-07 11:52:56.000000 dimples-0.1.8/dimples/station/shared.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3782 2023-06-04 10:23:09.000000 dimples-0.1.8/dimples/station/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/utils/
--rw-r--r--   0 moky       (501) staff       (20)     2568 2023-02-23 13:38:40.000000 dimples-0.1.8/dimples/utils/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6447 2022-12-22 12:24:04.000000 dimples-0.1.8/dimples/utils/cache.py
--rw-r--r--   0 moky       (501) staff       (20)     4016 2023-06-02 18:00:31.000000 dimples-0.1.8/dimples/utils/checker.py
--rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/utils/dos.py
--rw-r--r--   0 moky       (501) staff       (20)     2805 2022-12-28 05:23:15.000000 dimples-0.1.8/dimples/utils/log.py
--rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/utils/singleton.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)     3274 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)      118 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples.egg-info/entry_points.txt
--rw-r--r--   0 moky       (501) staff       (20)      108 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        8 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2023-06-12 15:42:23.000000 dimples-0.1.8/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)     1675 2023-06-12 09:37:23.000000 dimples-0.1.8/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:05.000000 dimples-0.2.0/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2023-06-18 14:42:05.000000 dimples-0.2.0/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-0.2.0/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples/
+-rw-r--r--   0 moky       (501) staff       (20)     7204 2023-06-18 14:35:59.000000 dimples-0.2.0/dimples/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples/client/
+-rw-r--r--   0 moky       (501) staff       (20)     1997 2023-06-03 11:38:39.000000 dimples-0.2.0/dimples/client/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples/client/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     2191 2023-06-09 16:37:34.000000 dimples-0.2.0/dimples/client/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4011 2023-06-02 18:30:20.000000 dimples-0.2.0/dimples/client/cpu/grp_expel.py
+-rw-r--r--   0 moky       (501) staff       (20)     4116 2023-06-02 18:31:07.000000 dimples-0.2.0/dimples/client/cpu/grp_invite.py
+-rw-r--r--   0 moky       (501) staff       (20)     3554 2023-02-23 11:18:06.000000 dimples-0.2.0/dimples/client/cpu/grp_query.py
+-rw-r--r--   0 moky       (501) staff       (20)     3558 2023-06-02 18:31:36.000000 dimples-0.2.0/dimples/client/cpu/grp_quit.py
+-rw-r--r--   0 moky       (501) staff       (20)     6498 2023-06-02 18:32:15.000000 dimples-0.2.0/dimples/client/cpu/grp_reset.py
+-rw-r--r--   0 moky       (501) staff       (20)     5150 2023-02-23 14:17:47.000000 dimples-0.2.0/dimples/client/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     2948 2023-01-31 05:28:07.000000 dimples-0.2.0/dimples/client/cpu/history.py
+-rw-r--r--   0 moky       (501) staff       (20)     1869 2023-01-31 05:28:07.000000 dimples-0.2.0/dimples/client/cpu/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     1847 2023-01-31 05:28:07.000000 dimples-0.2.0/dimples/client/cpu/receipt.py
+-rw-r--r--   0 moky       (501) staff       (20)     1895 2023-06-09 16:41:36.000000 dimples-0.2.0/dimples/client/cpu/text.py
+-rw-r--r--   0 moky       (501) staff       (20)    16324 2023-06-02 17:03:56.000000 dimples-0.2.0/dimples/client/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     9951 2023-06-12 14:16:50.000000 dimples-0.2.0/dimples/client/messenger.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples/client/network/
+-rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-0.2.0/dimples/client/network/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6258 2023-02-23 14:14:03.000000 dimples-0.2.0/dimples/client/network/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     8302 2023-06-03 11:39:42.000000 dimples-0.2.0/dimples/client/network/state.py
+-rw-r--r--   0 moky       (501) staff       (20)     9531 2023-01-31 05:28:07.000000 dimples-0.2.0/dimples/client/network/transition.py
+-rw-r--r--   0 moky       (501) staff       (20)     6619 2023-06-12 13:22:46.000000 dimples-0.2.0/dimples/client/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     7190 2023-06-09 16:42:29.000000 dimples-0.2.0/dimples/client/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5521 2023-02-23 14:13:41.000000 dimples-0.2.0/dimples/client/terminal.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples/common/
+-rw-r--r--   0 moky       (501) staff       (20)     2235 2023-06-18 14:35:34.000000 dimples-0.2.0/dimples/common/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     5559 2023-06-18 11:38:34.000000 dimples-0.2.0/dimples/common/ans.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples/common/dbi/
+-rw-r--r--   0 moky       (501) staff       (20)     2324 2023-06-09 14:20:27.000000 dimples-0.2.0/dimples/common/dbi/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6396 2023-06-02 10:33:41.000000 dimples-0.2.0/dimples/common/dbi/account.py
+-rw-r--r--   0 moky       (501) staff       (20)     2465 2023-06-02 07:39:55.000000 dimples-0.2.0/dimples/common/dbi/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     7877 2023-06-09 15:01:59.000000 dimples-0.2.0/dimples/common/dbi/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6739 2023-06-02 09:05:19.000000 dimples-0.2.0/dimples/common/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     7827 2023-06-12 14:51:01.000000 dimples-0.2.0/dimples/common/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     7710 2023-06-12 13:20:42.000000 dimples-0.2.0/dimples/common/packer.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples/common/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     2536 2023-06-18 14:35:34.000000 dimples-0.2.0/dimples/common/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3321 2023-06-09 16:01:10.000000 dimples-0.2.0/dimples/common/protocol/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     5004 2022-12-23 07:24:37.000000 dimples-0.2.0/dimples/common/protocol/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4523 2023-06-02 08:11:42.000000 dimples-0.2.0/dimples/common/protocol/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     6085 2023-06-02 08:40:15.000000 dimples-0.2.0/dimples/common/protocol/receipt.py
+-rw-r--r--   0 moky       (501) staff       (20)     2521 2023-06-02 08:42:45.000000 dimples-0.2.0/dimples/common/protocol/report.py
+-rw-r--r--   0 moky       (501) staff       (20)     4486 2023-06-04 16:41:38.000000 dimples-0.2.0/dimples/common/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6211 2023-06-03 12:24:47.000000 dimples-0.2.0/dimples/config.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples/conn/
+-rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-0.2.0/dimples/conn/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10335 2023-06-07 13:23:28.000000 dimples-0.2.0/dimples/conn/gate.py
+-rw-r--r--   0 moky       (501) staff       (20)     9892 2023-01-31 05:28:07.000000 dimples-0.2.0/dimples/conn/gatekeeper.py
+-rw-r--r--   0 moky       (501) staff       (20)    10305 2023-01-14 13:25:42.000000 dimples-0.2.0/dimples/conn/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     7851 2023-02-23 09:10:59.000000 dimples-0.2.0/dimples/conn/mtp.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:05.000000 dimples-0.2.0/dimples/conn/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-0.2.0/dimples/conn/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8711 2022-12-11 05:07:49.000000 dimples-0.2.0/dimples/conn/protocol/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     8254 2022-12-11 05:07:49.000000 dimples-0.2.0/dimples/conn/protocol/ws.py
+-rw-r--r--   0 moky       (501) staff       (20)     5411 2023-02-23 09:10:59.000000 dimples-0.2.0/dimples/conn/queue.py
+-rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-0.2.0/dimples/conn/seeker.py
+-rw-r--r--   0 moky       (501) staff       (20)     5726 2023-06-02 09:57:33.000000 dimples-0.2.0/dimples/conn/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6991 2023-01-14 12:47:37.000000 dimples-0.2.0/dimples/conn/ws.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:05.000000 dimples-0.2.0/dimples/database/
+-rw-r--r--   0 moky       (501) staff       (20)     2560 2023-06-04 16:46:57.000000 dimples-0.2.0/dimples/database/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7000 2023-06-02 12:26:57.000000 dimples-0.2.0/dimples/database/account.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:05.000000 dimples-0.2.0/dimples/database/dos/
+-rw-r--r--   0 moky       (501) staff       (20)     1808 2023-06-05 05:13:02.000000 dimples-0.2.0/dimples/database/dos/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4071 2022-12-22 17:59:17.000000 dimples-0.2.0/dimples/database/dos/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     3769 2022-12-11 05:07:49.000000 dimples-0.2.0/dimples/database/dos/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     4232 2023-06-02 10:30:44.000000 dimples-0.2.0/dimples/database/dos/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     3141 2023-06-02 11:02:33.000000 dimples-0.2.0/dimples/database/dos/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2680 2022-12-22 17:58:13.000000 dimples-0.2.0/dimples/database/dos/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5630 2023-06-02 11:04:20.000000 dimples-0.2.0/dimples/database/dos/private.py
+-rw-r--r--   0 moky       (501) staff       (20)     8033 2023-06-09 14:40:24.000000 dimples-0.2.0/dimples/database/dos/station.py
+-rw-r--r--   0 moky       (501) staff       (20)     5625 2023-06-02 11:01:02.000000 dimples-0.2.0/dimples/database/dos/user.py
+-rw-r--r--   0 moky       (501) staff       (20)     3097 2022-12-13 10:56:52.000000 dimples-0.2.0/dimples/database/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     4229 2023-06-04 17:05:32.000000 dimples-0.2.0/dimples/database/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     2972 2023-01-31 05:28:07.000000 dimples-0.2.0/dimples/database/t_cipherkey.py
+-rw-r--r--   0 moky       (501) staff       (20)     3710 2023-06-09 14:19:20.000000 dimples-0.2.0/dimples/database/t_document.py
+-rw-r--r--   0 moky       (501) staff       (20)     7715 2023-06-05 05:41:56.000000 dimples-0.2.0/dimples/database/t_group.py
+-rw-r--r--   0 moky       (501) staff       (20)     3718 2023-06-09 14:19:56.000000 dimples-0.2.0/dimples/database/t_login.py
+-rw-r--r--   0 moky       (501) staff       (20)     5144 2022-12-22 18:03:37.000000 dimples-0.2.0/dimples/database/t_message.py
+-rw-r--r--   0 moky       (501) staff       (20)     3513 2023-06-05 05:36:10.000000 dimples-0.2.0/dimples/database/t_meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5589 2023-06-05 05:38:08.000000 dimples-0.2.0/dimples/database/t_private.py
+-rw-r--r--   0 moky       (501) staff       (20)     6647 2023-06-05 05:31:39.000000 dimples-0.2.0/dimples/database/t_station.py
+-rw-r--r--   0 moky       (501) staff       (20)     6455 2023-06-05 05:39:18.000000 dimples-0.2.0/dimples/database/t_user.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:05.000000 dimples-0.2.0/dimples/edge/
+-rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-0.2.0/dimples/edge/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    13567 2023-06-12 14:07:59.000000 dimples-0.2.0/dimples/edge/octopus.py
+-rw-r--r--   0 moky       (501) staff       (20)     5594 2023-06-05 05:51:39.000000 dimples-0.2.0/dimples/edge/shared.py
+-rw-r--r--   0 moky       (501) staff       (20)     2726 2023-06-04 10:23:09.000000 dimples-0.2.0/dimples/edge/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:05.000000 dimples-0.2.0/dimples/register/
+-rw-r--r--   0 moky       (501) staff       (20)     1441 2022-12-11 05:07:49.000000 dimples-0.2.0/dimples/register/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     9516 2023-06-02 10:01:29.000000 dimples-0.2.0/dimples/register/generate.py
+-rw-r--r--   0 moky       (501) staff       (20)     7045 2023-06-02 10:02:10.000000 dimples-0.2.0/dimples/register/modify.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3880 2022-12-11 05:07:49.000000 dimples-0.2.0/dimples/register/run.py
+-rw-r--r--   0 moky       (501) staff       (20)     1971 2022-12-11 05:07:49.000000 dimples-0.2.0/dimples/register/shared.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:05.000000 dimples-0.2.0/dimples/server/
+-rw-r--r--   0 moky       (501) staff       (20)     2681 2023-06-18 09:57:24.000000 dimples-0.2.0/dimples/server/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8020 2023-06-18 10:50:18.000000 dimples-0.2.0/dimples/server/broadcast.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:05.000000 dimples-0.2.0/dimples/server/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     1855 2023-02-23 09:37:38.000000 dimples-0.2.0/dimples/server/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2668 2023-06-17 15:58:30.000000 dimples-0.2.0/dimples/server/cpu/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     4781 2023-06-03 12:02:30.000000 dimples-0.2.0/dimples/server/cpu/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     3464 2023-06-12 12:55:43.000000 dimples-0.2.0/dimples/server/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     3853 2023-06-03 12:02:46.000000 dimples-0.2.0/dimples/server/cpu/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     1847 2023-01-31 05:28:07.000000 dimples-0.2.0/dimples/server/cpu/receipt.py
+-rw-r--r--   0 moky       (501) staff       (20)     3089 2023-01-31 05:28:07.000000 dimples-0.2.0/dimples/server/cpu/report.py
+-rw-r--r--   0 moky       (501) staff       (20)    13588 2023-06-17 07:30:46.000000 dimples-0.2.0/dimples/server/dispatcher.py
+-rw-r--r--   0 moky       (501) staff       (20)     9473 2023-06-18 09:35:15.000000 dimples-0.2.0/dimples/server/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     6638 2023-06-18 11:45:32.000000 dimples-0.2.0/dimples/server/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     5791 2023-02-23 11:39:56.000000 dimples-0.2.0/dimples/server/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5448 2023-06-18 14:36:35.000000 dimples-0.2.0/dimples/server/push.py
+-rw-r--r--   0 moky       (501) staff       (20)     7978 2023-06-16 11:57:03.000000 dimples-0.2.0/dimples/server/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-0.2.0/dimples/server/session_center.py
+-rw-r--r--   0 moky       (501) staff       (20)     9704 2023-06-18 10:50:13.000000 dimples-0.2.0/dimples/server/trace.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:05.000000 dimples-0.2.0/dimples/station/
+-rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-0.2.0/dimples/station/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4624 2023-06-07 12:21:10.000000 dimples-0.2.0/dimples/station/handler.py
+-rw-r--r--   0 moky       (501) staff       (20)     6089 2023-06-18 11:39:31.000000 dimples-0.2.0/dimples/station/shared.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3708 2023-06-18 11:31:20.000000 dimples-0.2.0/dimples/station/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:05.000000 dimples-0.2.0/dimples/utils/
+-rw-r--r--   0 moky       (501) staff       (20)     2568 2023-02-23 13:38:40.000000 dimples-0.2.0/dimples/utils/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6446 2023-06-18 10:21:27.000000 dimples-0.2.0/dimples/utils/cache.py
+-rw-r--r--   0 moky       (501) staff       (20)     4016 2023-06-02 18:00:31.000000 dimples-0.2.0/dimples/utils/checker.py
+-rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-0.2.0/dimples/utils/dos.py
+-rw-r--r--   0 moky       (501) staff       (20)     2805 2022-12-28 05:23:15.000000 dimples-0.2.0/dimples/utils/log.py
+-rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-0.2.0/dimples/utils/singleton.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)     3265 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)      118 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples.egg-info/entry_points.txt
+-rw-r--r--   0 moky       (501) staff       (20)      108 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        8 2023-06-18 14:42:04.000000 dimples-0.2.0/dimples.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2023-06-18 14:42:05.000000 dimples-0.2.0/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)     1675 2023-06-16 08:07:02.000000 dimples-0.2.0/setup.py
```

### Comparing `dimples-0.1.8/PKG-INFO` & `dimples-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.1.8
+Version: 0.2.0
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.1.8/README.md` & `dimples-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/__init__.py` & `dimples-0.2.0/dimples/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/client/__init__.py` & `dimples-0.2.0/dimples/client/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/client/cpu/__init__.py` & `dimples-0.2.0/dimples/client/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/client/cpu/grp_expel.py` & `dimples-0.2.0/dimples/client/cpu/grp_expel.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/client/cpu/grp_invite.py` & `dimples-0.2.0/dimples/client/cpu/grp_invite.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/client/cpu/grp_query.py` & `dimples-0.2.0/dimples/client/cpu/grp_query.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/client/cpu/grp_quit.py` & `dimples-0.2.0/dimples/client/cpu/grp_quit.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/client/cpu/grp_reset.py` & `dimples-0.2.0/dimples/client/cpu/grp_reset.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/client/cpu/handshake.py` & `dimples-0.2.0/dimples/client/cpu/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/client/cpu/history.py` & `dimples-0.2.0/dimples/client/cpu/history.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/client/cpu/login.py` & `dimples-0.2.0/dimples/client/cpu/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/client/cpu/receipt.py` & `dimples-0.2.0/dimples/client/cpu/receipt.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/client/cpu/text.py` & `dimples-0.2.0/dimples/client/cpu/text.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/client/group.py` & `dimples-0.2.0/dimples/client/group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/client/messenger.py` & `dimples-0.2.0/dimples/client/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/client/network/__init__.py` & `dimples-0.2.0/dimples/client/network/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/client/network/session.py` & `dimples-0.2.0/dimples/client/network/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/client/network/state.py` & `dimples-0.2.0/dimples/client/network/state.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/client/network/transition.py` & `dimples-0.2.0/dimples/client/network/transition.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/client/packer.py` & `dimples-0.2.0/dimples/client/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/client/processor.py` & `dimples-0.2.0/dimples/client/processor.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/client/terminal.py` & `dimples-0.2.0/dimples/client/terminal.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/common/__init__.py` & `dimples-0.2.0/dimples/common/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     ~~~~~~~~~~~~~
 
 """
 
 from .protocol import *
 from .dbi import *
 
-from .ans import AddressNameServer
+from .ans import AddressNameServer, ANSFactory
 from .facebook import CommonFacebook
 from .messenger import CommonMessenger
 from .packer import CommonMessagePacker
 from .session import Transmitter, Session
 
 
 __all__ = [
@@ -62,14 +62,14 @@
     'LoginDBI', 'ProviderDBI', 'StationDBI',
     'SessionDBI',
     'ProviderInfo', 'StationInfo',
 
     #
     #   common
     #
-    'AddressNameServer',
+    'AddressNameServer', 'ANSFactory',
     'CommonFacebook',
     'CommonMessenger',
     'CommonMessagePacker',
     'Transmitter',
     'Session',
 ]
```

### Comparing `dimples-0.1.8/dimples/common/ans.py` & `dimples-0.2.0/dimples/common/ans.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     ~~~~~~~~~~~~~~~~~~~~
 
     A map for short name to ID, just like DNS
 """
 
 from typing import Optional, List, Dict
 
-from dimsdk import ID
+from dimsdk import Address, ID, IDFactory
 from dimsdk import ANYONE, EVERYONE, FOUNDER
 from dimsdk import AddressNameService
 
 
 class AddressNameServer(AddressNameService):
 
     def __init__(self):
@@ -105,17 +105,51 @@
         if self.cache(name=name, identifier=identifier):
             # TODO: save new record into database
             return True
 
     def fix(self, records: Dict[str, str]) -> int:
         """ remove the keywords temporary before save new records """
         count = 0
+        self.__reserved['apns'] = False
+        self.__reserved['master'] = False
+        self.__reserved['archivist'] = False
         self.__reserved['assistant'] = False
         # self.__reserved['station'] = False
         for alias in records:
-            identifier = ID.parse(identifier=records[alias])
-            assert identifier is not None, 'record error: %s => %s' % (alias, records[alias])
+            value = records[alias]
+            if value is None or len(value) == 0:
+                continue
+            identifier = ID.parse(identifier=value)
+            assert identifier is not None, 'record error: %s => %s' % (alias, value)
             if self.save(name=alias, identifier=identifier):
                 count += 1
         # self.__reserved['station'] = True
         self.__reserved['assistant'] = True
+        self.__reserved['archivist'] = True
+        self.__reserved['master'] = True
+        self.__reserved['apns'] = True
         return count
+
+
+class ANSFactory(IDFactory):
+
+    def __init__(self, factory: IDFactory, ans: AddressNameServer):
+        super().__init__()
+        self.__origin = factory
+        self.__ans = ans
+
+    # Override
+    def generate_id(self, meta, network: int, terminal: Optional[str] = None) -> ID:
+        return self.__origin.generate_id(meta=meta, network=network, terminal=terminal)
+
+    # Override
+    def create_id(self, name: Optional[str], address: Address, terminal: Optional[str] = None) -> ID:
+        return self.__origin.create_id(address=address, name=name, terminal=terminal)
+
+    # Override
+    def parse_id(self, identifier: str) -> Optional[ID]:
+        # try ANS record
+        aid = self.__ans.identifier(name=identifier)
+        if aid is None:
+            # parse by original factory
+            aid = self.__origin.parse_id(identifier=identifier)
+        return aid
```

### Comparing `dimples-0.1.8/dimples/common/dbi/__init__.py` & `dimples-0.2.0/dimples/common/dbi/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/common/dbi/account.py` & `dimples-0.2.0/dimples/common/dbi/account.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/common/dbi/message.py` & `dimples-0.2.0/dimples/common/dbi/message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/common/dbi/session.py` & `dimples-0.2.0/dimples/common/dbi/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/common/facebook.py` & `dimples-0.2.0/dimples/common/facebook.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/common/messenger.py` & `dimples-0.2.0/dimples/common/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/common/packer.py` & `dimples-0.2.0/dimples/common/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/common/protocol/__init__.py` & `dimples-0.2.0/dimples/common/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/common/protocol/ans.py` & `dimples-0.2.0/dimples/common/protocol/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/common/protocol/handshake.py` & `dimples-0.2.0/dimples/common/protocol/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/common/protocol/login.py` & `dimples-0.2.0/dimples/common/protocol/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/common/protocol/receipt.py` & `dimples-0.2.0/dimples/common/protocol/receipt.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/common/protocol/report.py` & `dimples-0.2.0/dimples/common/protocol/report.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/common/session.py` & `dimples-0.2.0/dimples/common/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/config.py` & `dimples-0.2.0/dimples/config.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/conn/__init__.py` & `dimples-0.2.0/dimples/conn/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/conn/gate.py` & `dimples-0.2.0/dimples/conn/gate.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/conn/gatekeeper.py` & `dimples-0.2.0/dimples/conn/gatekeeper.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/conn/mars.py` & `dimples-0.2.0/dimples/conn/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/conn/mtp.py` & `dimples-0.2.0/dimples/conn/mtp.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/conn/protocol/__init__.py` & `dimples-0.2.0/dimples/conn/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/conn/protocol/mars.py` & `dimples-0.2.0/dimples/conn/protocol/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/conn/protocol/ws.py` & `dimples-0.2.0/dimples/conn/protocol/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/conn/queue.py` & `dimples-0.2.0/dimples/conn/queue.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/conn/seeker.py` & `dimples-0.2.0/dimples/conn/seeker.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/conn/session.py` & `dimples-0.2.0/dimples/conn/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/conn/ws.py` & `dimples-0.2.0/dimples/conn/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/database/__init__.py` & `dimples-0.2.0/dimples/database/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/database/account.py` & `dimples-0.2.0/dimples/database/account.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/database/dos/__init__.py` & `dimples-0.2.0/dimples/database/dos/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/database/dos/base.py` & `dimples-0.2.0/dimples/database/dos/base.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/database/dos/document.py` & `dimples-0.2.0/dimples/database/dos/document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/database/dos/group.py` & `dimples-0.2.0/dimples/database/dos/group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/database/dos/login.py` & `dimples-0.2.0/dimples/database/dos/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/database/dos/meta.py` & `dimples-0.2.0/dimples/database/dos/meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/database/dos/private.py` & `dimples-0.2.0/dimples/database/dos/private.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/database/dos/station.py` & `dimples-0.2.0/dimples/database/dos/station.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/database/dos/user.py` & `dimples-0.2.0/dimples/database/dos/user.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/database/message.py` & `dimples-0.2.0/dimples/database/message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/database/session.py` & `dimples-0.2.0/dimples/database/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/database/t_cipherkey.py` & `dimples-0.2.0/dimples/database/t_cipherkey.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/database/t_document.py` & `dimples-0.2.0/dimples/database/t_document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/database/t_group.py` & `dimples-0.2.0/dimples/database/t_group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/database/t_login.py` & `dimples-0.2.0/dimples/database/t_login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/database/t_message.py` & `dimples-0.2.0/dimples/database/t_message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/database/t_meta.py` & `dimples-0.2.0/dimples/database/t_meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/database/t_private.py` & `dimples-0.2.0/dimples/database/t_private.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/database/t_station.py` & `dimples-0.2.0/dimples/database/t_station.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/database/t_user.py` & `dimples-0.2.0/dimples/database/t_user.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/edge/__init__.py` & `dimples-0.2.0/dimples/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/edge/octopus.py` & `dimples-0.2.0/dimples/edge/octopus.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/edge/shared.py` & `dimples-0.2.0/dimples/edge/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/edge/start.py` & `dimples-0.2.0/dimples/edge/start.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/register/__init__.py` & `dimples-0.2.0/dimples/register/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/register/generate.py` & `dimples-0.2.0/dimples/register/generate.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/register/modify.py` & `dimples-0.2.0/dimples/register/modify.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/register/run.py` & `dimples-0.2.0/dimples/register/run.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/register/shared.py` & `dimples-0.2.0/dimples/register/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/server/__init__.py` & `dimples-0.2.0/dimples/server/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,21 +30,25 @@
 """
 
 from .cpu import *
 
 from .session import ServerSession
 from .session_center import SessionCenter  # SessionPool
 
-from .push_info import PushAlert, PushInfo
-from .push_service import PushService, PushCenter
-from .pusher import Pusher, DefaultPusher
+from .broadcast import BroadcastRecipientManager
+
+from .push import BadgeKeeper, PushService
+from .push import PushCenter
 
 # from .dispatcher import Roamer, MessageDeliver, DeliverWorker
 from .dispatcher import Dispatcher
 
+from .trace import TraceNode, TraceList
+from .trace import TraceManager
+
 from .packer import BlockFilter, MuteFilter, FilterManager
 
 from .packer import ServerMessagePacker
 from .processor import ServerMessageProcessor, ServerContentProcessorCreator
 from .messenger import ServerMessenger
 
 
@@ -55,22 +59,28 @@
     #
     'HandshakeCommandProcessor', 'LoginCommandProcessor', 'ReportCommandProcessor',
     'AnsCommandProcessor', 'DocumentCommandProcessor', 'ReceiptCommandProcessor',
 
     # Session
     'ServerSession', 'SessionCenter',  # 'SessionPool',
 
+    'BroadcastRecipientManager',
+
     # Push Notification
-    'PushAlert', 'PushInfo', 'PushService', 'PushCenter',
-    'Pusher', 'DefaultPusher',
+    'BadgeKeeper', 'PushService',
+    'PushCenter',
 
     # Dispatcher
     # 'Roamer', 'MessageDeliver', 'DeliverWorker',
     'Dispatcher',
 
+    # Trace
+    'TraceNode', 'TraceList',
+    'TraceManager',
+
     # Filter
     'BlockFilter', 'MuteFilter', 'FilterManager',
 
     'ServerMessagePacker',
     'ServerMessageProcessor', 'ServerContentProcessorCreator',
     'ServerMessenger',
 ]
```

### Comparing `dimples-0.1.8/dimples/server/cpu/__init__.py` & `dimples-0.2.0/dimples/server/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/server/cpu/ans.py` & `dimples-0.2.0/dimples/server/cpu/ans.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,40 +34,40 @@
 
 from dimp import ID
 from dimp import ReliableMessage
 from dimp import Content
 
 from dimsdk.cpu import BaseCommandProcessor
 
-from ...utils import Log, Logging
+from ...utils import Log
 from ...common import AnsCommand
 
 
-class AnsCommandProcessor(BaseCommandProcessor, Logging):
+class AnsCommandProcessor(BaseCommandProcessor):
 
     # Override
     def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, AnsCommand), 'report command error: %s' % content
         names = content.names
         if names is None or len(names) == 0:
             text = 'ANS command error'
             return self._respond_text(text=text)
         records = {}
         missed = []
         for item in names:
             # get record from ANS factory
-            identifier = ans_id(name=item)
+            identifier = self.ans_id(name=item)
             if identifier is None:
                 missed.append(item)
             else:
                 records[item] = str(identifier)
         res = AnsCommand.response(names=names, records=records)
         if len(missed) > 0:
             res['missed'] = missed
         return [res]
 
-
-def ans_id(name: str) -> Optional[ID]:
-    try:
-        return ID.parse(identifier=name)
-    except ValueError as e:
-        Log.warning(msg='ANS record not exists: %s, %s' % (name, e))
+    @classmethod
+    def ans_id(cls, name: str) -> Optional[ID]:
+        try:
+            return ID.parse(identifier=name)
+        except ValueError as e:
+            Log.warning(msg='ANS record not exists: %s, %s' % (name, e))
```

### Comparing `dimples-0.1.8/dimples/server/cpu/document.py` & `dimples-0.2.0/dimples/server/cpu/document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/server/cpu/handshake.py` & `dimples-0.2.0/dimples/server/cpu/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/server/cpu/login.py` & `dimples-0.2.0/dimples/server/cpu/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/server/cpu/receipt.py` & `dimples-0.2.0/dimples/server/cpu/receipt.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/server/cpu/report.py` & `dimples-0.2.0/dimples/server/cpu/report.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/server/dispatcher.py` & `dimples-0.2.0/dimples/server/dispatcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 from ..utils import Singleton, Logging, Runner
 from ..common import CommonFacebook
 from ..common import MessageDBI, SessionDBI
 from ..common import LoginCommand, ReceiptCommand
 
 from .session_center import SessionCenter
-from .pusher import Pusher
+from .push import PushCenter
 
 
 class MessageDeliver(ABC):
     """ Delegate for deliver message """
 
     @abstractmethod
     def deliver_message(self, msg: ReliableMessage, receiver: ID) -> List[Content]:
@@ -66,15 +66,14 @@
 class Dispatcher(MessageDeliver):
 
     def __init__(self):
         super().__init__()
         self.__facebook: Optional[CommonFacebook] = None
         self.__mdb: Optional[MessageDBI] = None
         self.__sdb: Optional[SessionDBI] = None
-        self.__pusher: Optional[Pusher] = None
         # actually deliver worker
         self.__worker: Optional[DeliverWorker] = None
         # roaming user receptionist
         self.__roamer: Optional[Roamer] = None
 
     @property
     def facebook(self) -> CommonFacebook:
@@ -101,54 +100,56 @@
         return self.__sdb
 
     @sdb.setter
     def sdb(self, db: SessionDBI):
         self.__sdb = db
 
     #
-    #   Push Notification service
+    #   Worker
     #
 
     @property
-    def pusher(self) -> Pusher:
-        return self.__pusher
-
-    @pusher.setter
-    def pusher(self, service: Pusher):
-        self.__pusher = service
-
-    @property
-    def worker(self):  # -> DeliverWorker:
-        return self.__worker
-
-    def start(self):
-        worker = DeliverWorker(database=self.__sdb, facebook=self.__facebook)
-        roamer = Roamer(database=self.__mdb)
-        self.__worker = worker
-        self.__roamer = roamer
-        roamer.start()
+    def deliver_worker(self):  # -> DeliverWorker:
+        worker = self.__worker
+        if worker is None:
+            db = self.sdb
+            facebook = self.facebook
+            assert db is not None and facebook is not None, 'dispatcher not initialized'
+            worker = DeliverWorker(database=db, facebook=facebook)
+            self.__worker = worker
+        return worker
 
     #
     #   Roamer
     #
 
+    @property
+    def roamer(self):  # -> Roamer
+        runner = self.__roamer
+        if runner is None:
+            db = self.mdb
+            assert db is not None, 'dispatcher not initialized'
+            runner = Roamer(database=db)
+            self.__roamer = runner
+            runner.start()
+        return runner
+
     def add_roaming(self, user: ID, station: ID) -> bool:
         """ Add roaming user with station """
-        roamer = self.__roamer
-        if roamer is not None:
-            return roamer.add_roaming(user=user, station=station)
+        roamer = self.roamer
+        return roamer.add_roaming(user=user, station=station)
 
     #
     #   Deliver
     #
 
     # Override
     def deliver_message(self, msg: ReliableMessage, receiver: ID) -> List[Content]:
         """ Deliver message to destination """
-        worker = self.__worker
+        worker = self.deliver_worker
         if receiver.type == EntityType.STATION:
             # message to other stations
             # station won't roam to other station, so just push for it directly
             responses = worker.redirect_message(msg=msg, neighbor=receiver)
         elif receiver.type == EntityType.BOT:
             # message to a bot
             # save message before trying to push
@@ -158,19 +159,16 @@
             # message to user
             # save message before trying to push
             self.__save_reliable_message(msg=msg, receiver=receiver)
             responses = worker.push_message(msg=msg, receiver=receiver)
             if responses is None:
                 # failed to push message, user not online and not roamed to other station,
                 # push notification for the receiver
-                pusher = self.__pusher
-                if pusher is None:
-                    self.warning(msg='pusher not set yet, drop notification for: %s' % receiver)
-                else:
-                    pusher.push_notification(msg=msg)
+                center = PushCenter()
+                center.push_notification(msg=msg)
         # OK
         if responses is None:
             # user not online, and not roaming to other station
             text = 'Message cached'
             res = ReceiptCommand.create(text=text, msg=msg)
             return [res]
         elif len(responses) == 0:
@@ -252,15 +250,15 @@
                 info.start_pos = start + limit
                 self.__append(info=info)
             elif cached_messages is None or len(cached_messages) == 0:
                 self.debug(msg='no cached message for this user: %s' % receiver)
                 return True
             # get deliver delegate for receiver
             dispatcher = Dispatcher()
-            worker = dispatcher.worker
+            worker = dispatcher.deliver_worker
             # deliver cached messages one by one
             for msg in cached_messages:
                 worker.push_message(msg=msg, receiver=receiver)
         except Exception as e:
             self.error(msg='process roaming user (%s => %s) error: %s' % (receiver, roaming, e))
         # return True to process next immediately
         return True
@@ -302,15 +300,15 @@
             cmd = ReceiptCommand.create(text=text, msg=msg)
             cmd['recipient'] = str(receiver)
             return [cmd]
         # 2. get roaming station
         roaming = get_roaming_station(receiver=receiver, database=self.database)
         if roaming is None:
             # login command not found
-            # return None to tell the pusher to push notification for it.
+            # return None to tell the push center to push notification for it.
             return None
         # 3. redirect message to roaming station
         return self.redirect_message(msg=msg, neighbor=roaming)
 
     def redirect_message(self, msg: ReliableMessage, neighbor: ID) -> Optional[List[Content]]:
         """
         Redirect message to neighbor station
@@ -324,15 +322,15 @@
         self.info(msg='redirect message %s => %s to neighbor station: %s' % (msg.sender, msg.receiver, neighbor))
         # 0. check current station
         current = self.facebook.current_user.identifier
         assert current.type == EntityType.STATION, 'current station ID error: %s' % current
         if neighbor == current:
             self.debug(msg='same destination: %s, msg %s => %s' % (neighbor, msg.sender, msg.receiver))
             # the user is roaming to current station, but it's not online now
-            # return None to tell the pusher to push notification for it.
+            # return None to tell the push center to push notification for it.
             return None
         # 1. try to push message to neighbor station directly
         if session_push(msg=msg, receiver=neighbor) > 0:
             text = 'Message redirected to neighbor station'
             cmd = ReceiptCommand.create(text=text, msg=msg)
             cmd['neighbor'] = str(neighbor)
             return [cmd]
@@ -358,15 +356,15 @@
     if session_push(msg=msg, receiver=bridge) > 0:
         text = 'Message redirected to neighbor station via the bridge'
         cmd = ReceiptCommand.create(text=text, msg=msg)
         cmd['neighbor'] = str(neighbor)
         return [cmd]
     else:
         # station bridge not found
-        # return an empty array to avoid calling pusher
+        # return an empty array to avoid calling push center
         return []
 
 
 def session_push(msg: ReliableMessage, receiver: ID) -> int:
     """ push message via active session(s) of receiver """
     success = 0
     center = SessionCenter()
```

### Comparing `dimples-0.1.8/dimples/server/messenger.py` & `dimples-0.2.0/dimples/server/messenger.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,32 +26,29 @@
 """
     Messenger for request handler in station
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
     Transform and send message
 """
 
-import threading
-import time
-from typing import Optional, Set, List
+from typing import Optional, List
 
-from dimsdk import EntityType, ID, EVERYONE
+from dimsdk import ID, ANYONE
 from dimsdk import Station
 from dimsdk import Envelope, Command, MetaCommand, DocumentCommand
 from dimsdk import InstantMessage
 from dimsdk import SecureMessage, ReliableMessage
 
-from ..utils import Singleton, Log, QueryFrequencyChecker
+from ..utils import QueryFrequencyChecker
 from ..common import HandshakeCommand
 from ..common import CommonMessenger
-from ..common import SessionDBI
 
 from .packer import FilterManager
 from .dispatcher import Dispatcher
-from .session_center import SessionCenter
+from .broadcast import broadcast_reliable_message
 
 
 class ServerMessenger(CommonMessenger):
 
     # Override
     def handshake_success(self):
         session = self.session
@@ -65,74 +62,45 @@
             try:
                 responses = self.process_reliable_message(msg=msg)
                 for res in responses:
                     self.send_reliable_message(msg=res, priority=1)
             except Exception as error:
                 self.error(msg='failed to process incoming message: %s' % error)
 
-    def __broadcast_reliable_message(self, msg: ReliableMessage, station: ID):
-        receiver = msg.receiver
-        db = self.session.database
-        # get other recipients
-        recipients = get_recipients(msg=msg, receiver=receiver, db=db)
-        if len(recipients) == 0:
-            self.warning('other recipients not found: %s' % receiver)
-            return 0
-        sender = msg.sender
-        # dispatch
-        dispatcher = Dispatcher()
-        for target in recipients:
-            assert not target.is_broadcast, 'recipient error: %s, %s' % (target, receiver)
-            if target == station:
-                self.error(msg='current station should not exists here: %s, %s' % (target, recipients))
-                continue
-            elif target == sender:
-                self.warning(msg='skip sender: %s, %s' % (target, recipients))
-                continue
-            dispatcher.deliver_message(msg=msg, receiver=target)
-
-            # TODO: after deliver to connected neighbors, the dispatcher will continue
-            #       delivering via station bridge, should we mark 'sent_neighbors' in
-            #       only one message to the bridge, let the bridge to separate for other
-            #       neighbors which not connect to this station directly?
-        # OK
-        self.info(msg='Broadcast message delivered: %s, sender: %s' % (recipients, sender))
-        return len(recipients)
-
-    def __broadcast_command(self, content: Command, receiver: ID):
+    def _broadcast_command(self, content: Command, receiver: ID):
         sid = self.facebook.current_user.identifier
         env = Envelope.create(sender=sid, receiver=receiver)
         i_msg = InstantMessage.create(head=env, body=content)
         # pack & deliver message
         s_msg = self.encrypt_message(msg=i_msg)
         r_msg = self.sign_message(msg=s_msg)
-        self.__broadcast_reliable_message(msg=r_msg, station=sid)
+        broadcast_reliable_message(msg=r_msg, station=sid)
 
     # Override
     def query_meta(self, identifier: ID) -> bool:
         checker = QueryFrequencyChecker()
         if not checker.meta_query_expired(identifier=identifier):
             # query not expired yet
             self.debug(msg='meta query not expired yet: %s' % identifier)
             return False
         self.info(msg='querying meta of %s from neighbor stations' % identifier)
         command = MetaCommand.query(identifier=identifier)
-        self.__broadcast_command(content=command, receiver=Station.EVERY)
+        self._broadcast_command(content=command, receiver=Station.EVERY)
         return True
 
     # Override
     def query_document(self, identifier: ID) -> bool:
         checker = QueryFrequencyChecker()
         if not checker.document_query_expired(identifier=identifier):
             # query not expired yet
             self.debug(msg='document query not expired yet: %s' % identifier)
             return False
         self.info(msg='querying document of %s from neighbor stations' % identifier)
         command = DocumentCommand.query(identifier=identifier)
-        self.__broadcast_command(content=command, receiver=Station.EVERY)
+        self._broadcast_command(content=command, receiver=Station.EVERY)
         return True
 
     # Override
     def query_members(self, identifier: ID) -> bool:
         # station will never process group info
         return True
 
@@ -180,25 +148,26 @@
             # maybe a meta command, document command, etc ...
             return s_msg
         elif receiver.is_broadcast:
             # if receiver == 'station@anywhere':
             #     it must be the first handshake without station ID;
             # if receiver == 'anyone@anywhere':
             #     it should be other plain message without encryption.
+            if receiver == Station.ANY or receiver == ANYONE:
+                return s_msg
+            # broadcast message (to neighbor stations, or station bots)
+            broadcast_reliable_message(msg=msg, station=sid)
             # if receiver.is_group:
             #     broadcast message to multiple destinations,
             #     current station is it's receiver too.
             if receiver.is_group:
-                # broadcast to neighbor stations
-                self.__broadcast_reliable_message(msg=msg, station=sid)
-            elif receiver == 'archivist@anywhere':
-                # forward to search bot
-                self.__broadcast_reliable_message(msg=msg, station=sid)
-                return None
-            return s_msg
+                return s_msg
+            # otherwise, this message should have been redirected
+            # e.g.: 'archivist@anywhere', 'apns@anywhere', 'master@anywhere'
+            return None
         elif receiver.is_group:
             self.error(msg='group message should not send to station: %s -> %s' % (sender, receiver))
             return None
         # 3. this message is not for current station,
         # deliver to the real receiver and respond to sender
         dispatcher = Dispatcher()
         responses = dispatcher.deliver_message(msg=msg, receiver=receiver)
@@ -240,94 +209,7 @@
             # respond to the bridge
             responses.append(msg)
         else:
             # this message is not respond to the bridge, the receiver may be
             # roaming to other station, so deliver it via dispatcher here.
             dispatcher.deliver_message(msg=msg, receiver=receiver)
     return responses
-
-
-def get_neighbors(db: SessionDBI) -> Set[ID]:
-    neighbors = set()
-    providers = db.all_providers()
-    assert len(providers) > 0, 'service provider not found'
-    gsp = providers[0].identifier
-    stations = db.all_stations(provider=gsp)
-    for item in stations:
-        sid = item.identifier
-        if sid is None or sid.is_broadcast:
-            continue
-        neighbors.add(sid)
-    # get neighbor station from session server
-    proactive_neighbors = NeighborSessionManager().proactive_neighbors
-    for sid in proactive_neighbors:
-        if sid is None or sid.is_broadcast:
-            assert False, 'neighbor station ID error: %s' % sid
-            # continue
-        neighbors.add(sid)
-    return neighbors
-
-
-@Singleton
-class NeighborSessionManager:
-
-    def __init__(self):
-        super().__init__()
-        self.__neighbors = set()
-        self.__expires = 0
-        self.__lock = threading.Lock()
-
-    @property
-    def proactive_neighbors(self) -> Set[ID]:
-        now = time.time()
-        with self.__lock:
-            if self.__expires < now:
-                neighbors = set()
-                center = SessionCenter()
-                all_users = center.all_users()
-                for item in all_users:
-                    if item.type == EntityType.STATION:
-                        neighbors.add(item)
-                self.__neighbors = neighbors
-                self.__expires = now + 128
-            return self.__neighbors
-
-
-def get_recipients(msg: ReliableMessage, receiver: ID, db: SessionDBI) -> Set[ID]:
-    recipients = set()
-    # get nodes passed through, includes current node which is just added before
-    traces = msg.get('traces')
-    if traces is None:
-        traces = []
-    # if this message is sending to 'stations@everywhere' or 'everyone@everywhere'
-    # get all neighbor stations to broadcast, but
-    # traced nodes should be ignored to avoid cycled delivering
-    if receiver == Station.EVERY or receiver == EVERYONE:
-        Log.info(msg='forward to neighbors: %s' % receiver)
-        # get neighbor stations
-        neighbors = get_neighbors(db=db)
-        for sid in neighbors:
-            if sid not in traces:  # and sid != station:
-                recipients.add(sid)
-            else:
-                Log.warning(msg='ignore neighbor: %s' % sid)
-        # get archivist bot
-        if receiver == EVERYONE:
-            # include 'archivist' as 'everyone@everywhere'
-            bot = ans_id(name='archivist')
-            if bot is not None and bot not in traces:
-                recipients.add(bot)
-    elif receiver == 'archivist@anywhere' or receiver == 'archivists@everywhere':
-        Log.info(msg='forward to archivist: %s' % receiver)
-        # get archivist bot for search command
-        bot = ans_id(name='archivist')
-        if bot is not None and bot not in traces:
-            recipients.add(bot)
-    Log.info(msg='recipients: %s -> %s' % (receiver, recipients))
-    return recipients
-
-
-def ans_id(name: str) -> Optional[ID]:
-    try:
-        return ID.parse(identifier=name)
-    except ValueError as e:
-        Log.warning(msg='ANS record not exists: %s, %s' % (name, e))
```

### Comparing `dimples-0.1.8/dimples/server/packer.py` & `dimples-0.2.0/dimples/server/packer.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,54 +24,42 @@
 # ==============================================================================
 
 """
     Common extensions for MessagePacker
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 
-from typing import Optional, Dict
+from typing import Optional
 
 from dimsdk import EntityType, ID
 from dimsdk import SecureMessage, ReliableMessage
 
 from ..utils import Singleton, Logging
 from ..common import CommonFacebook
 from ..common import CommonMessagePacker
 
+from .trace import TraceManager
+
 
 class ServerMessagePacker(CommonMessagePacker):
 
     def __current(self) -> ID:
         """ current station ID """
         facebook = get_facebook(packer=self)
         current = facebook.current_user
         sid = current.identifier
         assert sid is not None, 'current station error: %s' % current
         return sid
 
     def __is_traced(self, msg: ReliableMessage) -> bool:
-        is_traced = False
+        """ check & append current node in msg['traces'] """
         node = self.__current()
-        # check current node in msg['traces']
-        traces = msg.get('traces')
-        if traces is None:
-            # start from here
-            msg['traces'] = [str(node)]
-        else:
-            for item in traces:
-                if isinstance(item, Dict):
-                    sid = item.get('ID')
-                else:
-                    # assert isinstance(item, str), 'MTA error: %s' % item
-                    sid = item
-                if node == sid:
-                    is_traced = True
-                    break
-            # append current node to msg['traces']
-            traces.append(str(node))
+        tm = TraceManager()
+        is_traced = tm.is_traced(msg=msg, node=node)
+        tm.add_node(msg=msg, node=node)
         return is_traced
 
     def __is_trusted(self, sender: ID) -> bool:
         messenger = get_messenger(packer=self)
         session = messenger.session
         user = session.identifier
         if user is None:
@@ -177,9 +165,25 @@
 
 
 @Singleton
 class FilterManager:
 
     def __init__(self):
         super().__init__()
-        self.block_filter = BlockFilter()
-        self.mute_filter = MuteFilter()
+        self.__block_filter = BlockFilter()
+        self.__mute_filter = MuteFilter()
+
+    @property
+    def block_filter(self) -> BlockFilter:
+        return self.__block_filter
+
+    @block_filter.setter
+    def block_filter(self, delegate: BlockFilter):
+        self.__block_filter = delegate
+
+    @property
+    def mute_filter(self) -> MuteFilter:
+        return self.__mute_filter
+
+    @mute_filter.setter
+    def mute_filter(self, delegate: MuteFilter):
+        self.__mute_filter = delegate
```

### Comparing `dimples-0.1.8/dimples/server/processor.py` & `dimples-0.2.0/dimples/server/processor.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/server/session.py` & `dimples-0.2.0/dimples/server/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 from ..utils import hex_encode, random_bytes
 from ..utils import Log
 from ..common import SessionDBI
 from ..database import ReliableMessageTable
 from ..conn import BaseSession
 from ..conn import WSArrival, MarsStreamArrival, MTPStreamArrival
 
-from .push_service import PushCenter
+from .push import PushCenter
 
 
 def generate_session_key() -> str:
     """ generate random string """
     return hex_encode(random_bytes(32))
```

### Comparing `dimples-0.1.8/dimples/server/session_center.py` & `dimples-0.2.0/dimples/server/session_center.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/station/__init__.py` & `dimples-0.2.0/dimples/station/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/station/handler.py` & `dimples-0.2.0/dimples/station/handler.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/station/shared.py` & `dimples-0.2.0/dimples/station/shared.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,64 +23,38 @@
 # SOFTWARE.
 # ==============================================================================
 
 import getopt
 import sys
 from typing import Optional, Tuple
 
-from dimsdk import Address, ID, IDFactory
+from dimsdk import ID
 
 from ..utils import Singleton
-from ..common import AddressNameServer, CommonFacebook
+from ..common import AddressNameServer, ANSFactory, CommonFacebook
 from ..common import AccountDBI, MessageDBI, SessionDBI
 from ..common import ProviderInfo
 from ..database import AccountDatabase, MessageDatabase, SessionDatabase
 from ..database import Storage
-from ..server import Pusher, DefaultPusher, PushCenter
+from ..server import BroadcastRecipientManager
 from ..server import Dispatcher
 
 from ..config import Config
 
 
-class ANSFactory(IDFactory):
-
-    def __init__(self, factory: IDFactory, ans: AddressNameServer):
-        super().__init__()
-        self.__origin = factory
-        self.__ans = ans
-
-    # Override
-    def generate_id(self, meta, network: int, terminal: Optional[str] = None) -> ID:
-        return self.__origin.generate_id(meta=meta, network=network, terminal=terminal)
-
-    # Override
-    def create_id(self, name: Optional[str], address: Address, terminal: Optional[str] = None) -> ID:
-        return self.__origin.create_id(address=address, name=name, terminal=terminal)
-
-    # Override
-    def parse_id(self, identifier: str) -> Optional[ID]:
-        # try ANS record
-        aid = self.__ans.identifier(name=identifier)
-        if aid is None:
-            # parse by original factory
-            aid = self.__origin.parse_id(identifier=identifier)
-        return aid
-
-
 @Singleton
 class GlobalVariable:
 
     def __init__(self):
         super().__init__()
         self.config: Optional[Config] = None
         self.adb: Optional[AccountDBI] = None
         self.mdb: Optional[MessageDBI] = None
         self.sdb: Optional[SessionDBI] = None
         self.facebook: Optional[CommonFacebook] = None
-        self.pusher: Optional[Pusher] = None
 
 
 def show_help(cmd: str, app_name: str, default_config: str):
     print('')
     print('    %s' % app_name)
     print('')
     print('usages:')
@@ -157,39 +131,34 @@
     assert sign_key is not None, 'failed to get sign key for current user: %s' % current_user
     assert msg_keys is not None and len(msg_keys) > 0, 'failed to get msg keys: %s' % current_user
     print('set current user: %s' % current_user)
     facebook.current_user = facebook.user(identifier=current_user)
     return facebook
 
 
+def create_dispatcher(shared: GlobalVariable) -> Dispatcher:
+    """ Step 4: create dispatcher """
+    dispatcher = Dispatcher()
+    dispatcher.mdb = shared.mdb
+    dispatcher.sdb = shared.sdb
+    dispatcher.facebook = shared.facebook
+    return dispatcher
+
+
 def create_ans(config: Config) -> AddressNameServer:
-    """ Step 4: create ANS """
+    """ Step 5: create ANS """
     ans = AddressNameServer()
     factory = ID.factory()
     ID.register(factory=ANSFactory(factory=factory, ans=ans))
     # load ANS records from 'config.ini'
     ans_records = config.ans_records
     if ans_records is not None:
         ans.fix(records=ans_records)
+    # set bots to receive message for 'everyone@everywhere'
+    bots = set()
+    se = ans.identifier(name='archivist')  # Search Engine
+    if se is not None:
+        bots.add(se)
+    if len(bots) > 0:
+        manager = BroadcastRecipientManager()
+        manager.station_bots = bots
     return ans
-
-
-def create_pusher(shared: GlobalVariable) -> Pusher:
-    """ Step 5: create pusher """
-    pusher = DefaultPusher(facebook=shared.facebook)
-    shared.pusher = pusher
-    # start PushCenter
-    center = PushCenter()
-    # TODO: add push services
-    center.start()
-    return pusher
-
-
-def create_dispatcher(shared: GlobalVariable) -> Dispatcher:
-    """ Step 6: create dispatcher """
-    dispatcher = Dispatcher()
-    dispatcher.mdb = shared.mdb
-    dispatcher.sdb = shared.sdb
-    dispatcher.facebook = shared.facebook
-    dispatcher.pusher = shared.pusher
-    dispatcher.start()
-    return dispatcher
```

### Comparing `dimples-0.1.8/dimples/station/start.py` & `dimples-0.2.0/dimples/station/start.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,23 +40,23 @@
 path = os.path.dirname(path)
 sys.path.insert(0, path)
 
 from dimples.utils import Log
 
 from dimples.station.shared import GlobalVariable
 from dimples.station.shared import create_config, create_database, create_facebook
-from dimples.station.shared import create_ans, create_pusher
 from dimples.station.shared import create_dispatcher
+from dimples.station.shared import create_ans
 from dimples.station.handler import RequestHandler
 
 
 #
 # show logs
 #
-Log.LEVEL = Log.DEBUG
+Log.LEVEL = Log.DEVELOP
 
 
 DEFAULT_CONFIG = '/etc/dim/station.ini'
 
 
 def main():
     # create global variable
@@ -70,20 +70,18 @@
     shared.mdb = mdb
     shared.sdb = sdb
     # Step 3: create facebook
     sid = config.station_id
     assert sid is not None, 'current station ID not set: %s' % config
     facebook = create_facebook(database=adb, current_user=sid)
     shared.facebook = facebook
-    # Step 4: create ANS
-    create_ans(config=config)
-    # Step 5: create pusher
-    create_pusher(shared=shared)
-    # Step 6: create dispatcher
+    # Step 4: create dispatcher
     create_dispatcher(shared=shared)
+    # Step 5: create ANS
+    create_ans(config=config)
     # check bind host & port
     host = config.station_host
     port = config.station_port
     assert host is not None and port > 0, 'station config error: %s' % config
     server_address = (host, port)
 
     # start TCP server
```

### Comparing `dimples-0.1.8/dimples/utils/__init__.py` & `dimples-0.2.0/dimples/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/utils/cache.py` & `dimples-0.2.0/dimples/utils/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,13 +187,13 @@
             pool = CachePool()
             self.__pools[name] = pool
         return pool
 
     def purge(self, now: float) -> int:
         """ purge all pools """
         count = 0
-        names = list(self.__pools.keys())
+        names = set(self.__pools.keys())
         for name in names:
             pool = self.__pools.get(name)
             if pool is not None:
                 count += pool.purge(now=now)
         return count
```

### Comparing `dimples-0.1.8/dimples/utils/checker.py` & `dimples-0.2.0/dimples/utils/checker.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/utils/dos.py` & `dimples-0.2.0/dimples/utils/dos.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/utils/log.py` & `dimples-0.2.0/dimples/utils/log.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples/utils/singleton.py` & `dimples-0.2.0/dimples/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.8/dimples.egg-info/PKG-INFO` & `dimples-0.2.0/dimples.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.1.8
+Version: 0.2.0
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.1.8/dimples.egg-info/SOURCES.txt` & `dimples-0.2.0/dimples.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -85,23 +85,23 @@
 dimples/edge/start.py
 dimples/register/__init__.py
 dimples/register/generate.py
 dimples/register/modify.py
 dimples/register/run.py
 dimples/register/shared.py
 dimples/server/__init__.py
+dimples/server/broadcast.py
 dimples/server/dispatcher.py
 dimples/server/messenger.py
 dimples/server/packer.py
 dimples/server/processor.py
-dimples/server/push_info.py
-dimples/server/push_service.py
-dimples/server/pusher.py
+dimples/server/push.py
 dimples/server/session.py
 dimples/server/session_center.py
+dimples/server/trace.py
 dimples/server/cpu/__init__.py
 dimples/server/cpu/ans.py
 dimples/server/cpu/document.py
 dimples/server/cpu/handshake.py
 dimples/server/cpu/login.py
 dimples/server/cpu/receipt.py
 dimples/server/cpu/report.py
```

### Comparing `dimples-0.1.8/setup.py` & `dimples-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     communications between accounts safely by end-to-end encryption.
 """
 
 import io
 
 from setuptools import setup, find_packages
 
-__version__ = '0.1.8'
+__version__ = '0.2.0'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     readme = fh.read()
 
 setup(
```

