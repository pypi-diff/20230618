# Comparing `tmp/bupap-0.1.0.tar.gz` & `tmp/bupap-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bupap-0.1.0.tar", max compression
+gzip compressed data, was "bupap-0.1.1.tar", max compression
```

## Comparing `bupap-0.1.0.tar` & `bupap-0.1.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0    34523 2023-06-11 08:29:21.399437 bupap-0.1.0/LICENSE
--rw-r--r--   0        0        0       71 2023-06-09 10:44:51.223117 bupap-0.1.0/README.md
--rw-r--r--   0        0        0     1365 2023-06-11 10:42:01.257060 bupap-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-26 13:35:02.277773 bupap-0.1.0/src/bupap/__init__.py
--rw-r--r--   0        0        0      349 2023-06-11 09:02:32.851063 bupap-0.1.0/src/bupap/avatar.py
--rw-r--r--   0        0        0     1089 2023-06-11 09:02:32.901065 bupap-0.1.0/src/bupap/config.py
--rw-r--r--   0        0        0     5271 2023-06-09 10:20:22.867696 bupap-0.1.0/src/bupap/data/bupap_avatar.svg
--rw-r--r--   0        0        0      291 2023-04-20 11:00:50.418356 bupap-0.1.0/src/bupap/db/__init__.py
--rw-r--r--   0        0        0       38 2023-03-27 17:21:17.549405 bupap-0.1.0/src/bupap/db/alembic/README
--rw-r--r--   0        0        0        0 2023-03-27 17:21:17.552738 bupap-0.1.0/src/bupap/db/alembic/__init__.py
--rw-r--r--   0        0        0     3333 2023-06-09 14:38:59.202815 bupap-0.1.0/src/bupap/db/alembic/alembic.ini
--rw-r--r--   0        0        0     1926 2023-06-09 10:19:05.057812 bupap-0.1.0/src/bupap/db/alembic/env.py
--rw-r--r--   0        0        0      510 2023-03-27 17:21:17.552738 bupap-0.1.0/src/bupap/db/alembic/script.py.mako
--rw-r--r--   0        0        0    21832 2023-06-11 09:02:33.361076 bupap-0.1.0/src/bupap/db/alembic/versions/2023-04-28_initial.py
--rw-r--r--   0        0        0        0 2023-03-27 17:21:17.552738 bupap-0.1.0/src/bupap/db/alembic/versions/__init__.py
--rw-r--r--   0        0        0     1604 2023-06-11 07:55:06.862579 bupap-0.1.0/src/bupap/db/database.py
--rw-r--r--   0        0        0     4583 2023-06-09 10:19:05.201146 bupap-0.1.0/src/bupap/db/defaults.py
--rw-r--r--   0        0        0      585 2023-06-05 17:27:41.576759 bupap-0.1.0/src/bupap/db/tables/__init__.py
--rw-r--r--   0        0        0      273 2023-04-21 07:48:23.202279 bupap-0.1.0/src/bupap/db/tables/assocs.py
--rw-r--r--   0        0        0     1749 2023-06-05 17:45:15.485511 bupap-0.1.0/src/bupap/db/tables/base.py
--rw-r--r--   0        0        0     2610 2023-05-15 17:22:30.306690 bupap-0.1.0/src/bupap/db/tables/estimate.py
--rw-r--r--   0        0        0      768 2023-05-29 10:29:20.875695 bupap-0.1.0/src/bupap/db/tables/history.py
--rw-r--r--   0        0        0     1032 2023-06-03 08:34:55.409568 bupap-0.1.0/src/bupap/db/tables/project.py
--rw-r--r--   0        0        0     2507 2023-06-09 10:19:05.444478 bupap-0.1.0/src/bupap/db/tables/role.py
--rw-r--r--   0        0        0     4104 2023-06-09 09:08:28.224413 bupap-0.1.0/src/bupap/db/tables/schedule.py
--rw-r--r--   0        0        0     2713 2023-05-29 10:39:01.886176 bupap-0.1.0/src/bupap/db/tables/task.py
--rw-r--r--   0        0        0      579 2023-04-21 07:48:23.252279 bupap-0.1.0/src/bupap/db/tables/team.py
--rw-r--r--   0        0        0     4089 2023-06-09 10:19:05.001146 bupap-0.1.0/src/bupap/db/tables/user.py
--rw-r--r--   0        0        0     2046 2023-06-05 17:43:31.022158 bupap-0.1.0/src/bupap/db/tables/work.py
--rw-r--r--   0        0        0    23268 2023-06-09 10:47:15.829788 bupap-0.1.0/src/bupap/db/testdata.py
--rw-r--r--   0        0        0      471 2023-06-11 09:02:32.917732 bupap-0.1.0/src/bupap/entrypoint/bupap_alembic.py
--rw-r--r--   0        0        0      436 2023-06-11 09:02:32.921065 bupap-0.1.0/src/bupap/entrypoint/bupap_settings.py
--rw-r--r--   0        0        0     3699 2023-06-11 10:37:36.184175 bupap-0.1.0/src/bupap/entrypoint/main.py
--rw-r--r--   0        0        0      336 2023-06-09 10:19:05.314478 bupap-0.1.0/src/bupap/injection.py
--rw-r--r--   0        0        0      882 2023-04-21 07:48:23.295613 bupap-0.1.0/src/bupap/log_config.py
--rw-r--r--   0        0        0     2007 2023-05-03 16:20:37.159834 bupap-0.1.0/src/bupap/permissions.py
--rw-r--r--   0        0        0      366 2023-06-10 15:33:55.586905 bupap-0.1.0/src/bupap/settings_default.toml
--rw-r--r--   0        0        0        0 2023-04-18 18:45:59.268532 bupap-0.1.0/src/bupap/ui/__init__.py
--rw-r--r--   0        0        0     1992 2023-06-09 10:19:05.517812 bupap-0.1.0/src/bupap/ui/common.py
--rw-r--r--   0        0        0      473 2023-05-09 18:16:06.277872 bupap-0.1.0/src/bupap/ui/component/__init__.py
--rw-r--r--   0        0        0     1970 2023-06-09 10:19:04.744480 bupap-0.1.0/src/bupap/ui/component/adduser.py
--rw-r--r--   0        0        0      468 2023-06-09 10:19:04.644480 bupap-0.1.0/src/bupap/ui/component/avatar.py
--rw-r--r--   0        0        0      596 2023-04-02 13:58:27.293968 bupap-0.1.0/src/bupap/ui/component/errors.js
--rw-r--r--   0        0        0     3960 2023-06-11 09:02:33.014401 bupap-0.1.0/src/bupap/ui/component/errors.py
--rw-r--r--   0        0        0     4702 2023-06-09 09:08:28.227746 bupap-0.1.0/src/bupap/ui/component/gantt.py
--rw-r--r--   0        0        0    12377 2023-06-03 11:16:21.540333 bupap-0.1.0/src/bupap/ui/component/gantt.vue
--rw-r--r--   0        0        0     1543 2023-06-09 10:19:04.471146 bupap-0.1.0/src/bupap/ui/component/header.py
--rw-r--r--   0        0        0     1283 2023-05-15 17:22:30.300023 bupap-0.1.0/src/bupap/ui/component/pick_date.py
--rw-r--r--   0        0        0     1300 2023-05-14 10:10:26.239776 bupap-0.1.0/src/bupap/ui/component/pick_date.vue
--rw-r--r--   0        0        0      824 2023-03-31 17:20:09.472334 bupap-0.1.0/src/bupap/ui/component/router.js
--rw-r--r--   0        0        0     5453 2023-06-09 10:19:04.354480 bupap-0.1.0/src/bupap/ui/component/router.py
--rw-r--r--   0        0        0      624 2023-06-09 10:19:04.287814 bupap-0.1.0/src/bupap/ui/component/user_card.py
--rw-r--r--   0        0        0        0 2023-04-19 12:08:19.926227 bupap-0.1.0/src/bupap/ui/crud/__init__.py
--rw-r--r--   0        0        0      759 2023-06-09 10:19:04.177814 bupap-0.1.0/src/bupap/ui/crud/common.py
--rw-r--r--   0        0        0     3283 2023-06-09 10:19:04.057814 bupap-0.1.0/src/bupap/ui/crud/project.py
--rw-r--r--   0        0        0    17461 2023-06-11 09:02:33.314408 bupap-0.1.0/src/bupap/ui/crud/task.py
--rw-r--r--   0        0        0     4573 2023-06-09 10:19:03.964480 bupap-0.1.0/src/bupap/ui/crud/team.py
--rw-r--r--   0        0        0     1069 2023-06-09 10:19:03.807814 bupap-0.1.0/src/bupap/ui/crud/user.py
--rw-r--r--   0        0        0     4686 2023-06-09 10:19:03.774481 bupap-0.1.0/src/bupap/ui/crud/work.py
--rw-r--r--   0        0        0      401 2023-05-01 11:06:05.700887 bupap-0.1.0/src/bupap/ui/page/__init__.py
--rw-r--r--   0        0        0     1352 2023-06-09 11:51:57.867329 bupap-0.1.0/src/bupap/ui/page/index.py
--rw-r--r--   0        0        0     1744 2023-06-09 11:52:02.273992 bupap-0.1.0/src/bupap/ui/page/login.py
--rw-r--r--   0        0        0     4476 2023-06-09 11:52:13.130650 bupap-0.1.0/src/bupap/ui/page/projects.py
--rw-r--r--   0        0        0    10847 2023-06-09 11:52:06.523988 bupap-0.1.0/src/bupap/ui/page/tasks.py
--rw-r--r--   0        0        0    12154 2023-06-09 11:52:16.193981 bupap-0.1.0/src/bupap/ui/page/teams.py
--rw-r--r--   0        0        0    16458 2023-06-09 11:52:19.503978 bupap-0.1.0/src/bupap/ui/page/users.py
--rw-r--r--   0        0        0      265 2023-04-20 18:26:08.662931 bupap-0.1.0/src/bupap/ui/viewmodel/__init__.py
--rw-r--r--   0        0        0      137 2023-04-21 07:48:23.412279 bupap-0.1.0/src/bupap/ui/viewmodel/login_information.py
--rw-r--r--   0        0        0      258 2023-06-09 10:19:02.994482 bupap-0.1.0/src/bupap/ui/viewmodel/project.py
--rw-r--r--   0        0        0      753 2023-06-09 10:19:02.974482 bupap-0.1.0/src/bupap/ui/viewmodel/task.py
--rw-r--r--   0        0        0      155 2023-06-09 10:19:02.964482 bupap-0.1.0/src/bupap/ui/viewmodel/team.py
--rw-r--r--   0        0        0      461 2023-06-09 10:19:02.961149 bupap-0.1.0/src/bupap/ui/viewmodel/user.py
--rw-r--r--   0        0        0      975 2023-06-09 10:19:02.957816 bupap-0.1.0/src/bupap/ui/viewmodel/work.py
--rw-r--r--   0        0        0     1179 1970-01-01 00:00:00.000000 bupap-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-11 08:29:21.399437 bupap-0.1.1/LICENSE
+-rw-r--r--   0        0        0      932 2023-06-18 11:53:04.290203 bupap-0.1.1/README.md
+-rw-r--r--   0        0        0     1324 2023-06-18 11:56:22.813228 bupap-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-26 13:35:02.277773 bupap-0.1.1/src/bupap/__init__.py
+-rw-r--r--   0        0        0      431 2023-06-17 22:33:02.435483 bupap-0.1.1/src/bupap/avatar.py
+-rw-r--r--   0        0        0     1175 2023-06-18 07:43:06.831719 bupap-0.1.1/src/bupap/config.py
+-rw-r--r--   0        0        0     5271 2023-06-09 10:20:22.867696 bupap-0.1.1/src/bupap/data/bupap_avatar.svg
+-rw-r--r--   0        0        0      291 2023-04-20 11:00:50.418356 bupap-0.1.1/src/bupap/db/__init__.py
+-rw-r--r--   0        0        0       38 2023-03-27 17:21:17.549405 bupap-0.1.1/src/bupap/db/alembic/README
+-rw-r--r--   0        0        0        0 2023-03-27 17:21:17.552738 bupap-0.1.1/src/bupap/db/alembic/__init__.py
+-rw-r--r--   0        0        0     3333 2023-06-09 14:38:59.202815 bupap-0.1.1/src/bupap/db/alembic/alembic.ini
+-rw-r--r--   0        0        0     1926 2023-06-09 10:19:05.057812 bupap-0.1.1/src/bupap/db/alembic/env.py
+-rw-r--r--   0        0        0      510 2023-03-27 17:21:17.552738 bupap-0.1.1/src/bupap/db/alembic/script.py.mako
+-rw-r--r--   0        0        0    21832 2023-06-11 09:02:33.361076 bupap-0.1.1/src/bupap/db/alembic/versions/2023-04-28_initial.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:21:17.552738 bupap-0.1.1/src/bupap/db/alembic/versions/__init__.py
+-rw-r--r--   0        0        0     1604 2023-06-11 07:55:06.862579 bupap-0.1.1/src/bupap/db/database.py
+-rw-r--r--   0        0        0     4583 2023-06-09 10:19:05.201146 bupap-0.1.1/src/bupap/db/defaults.py
+-rw-r--r--   0        0        0      585 2023-06-05 17:27:41.576759 bupap-0.1.1/src/bupap/db/tables/__init__.py
+-rw-r--r--   0        0        0      273 2023-04-21 07:48:23.202279 bupap-0.1.1/src/bupap/db/tables/assocs.py
+-rw-r--r--   0        0        0     1749 2023-06-05 17:45:15.485511 bupap-0.1.1/src/bupap/db/tables/base.py
+-rw-r--r--   0        0        0     2610 2023-05-15 17:22:30.306690 bupap-0.1.1/src/bupap/db/tables/estimate.py
+-rw-r--r--   0        0        0      768 2023-05-29 10:29:20.875695 bupap-0.1.1/src/bupap/db/tables/history.py
+-rw-r--r--   0        0        0     1032 2023-06-03 08:34:55.409568 bupap-0.1.1/src/bupap/db/tables/project.py
+-rw-r--r--   0        0        0     2507 2023-06-09 10:19:05.444478 bupap-0.1.1/src/bupap/db/tables/role.py
+-rw-r--r--   0        0        0     4104 2023-06-09 09:08:28.224413 bupap-0.1.1/src/bupap/db/tables/schedule.py
+-rw-r--r--   0        0        0     2713 2023-05-29 10:39:01.886176 bupap-0.1.1/src/bupap/db/tables/task.py
+-rw-r--r--   0        0        0      579 2023-04-21 07:48:23.252279 bupap-0.1.1/src/bupap/db/tables/team.py
+-rw-r--r--   0        0        0     4089 2023-06-09 10:19:05.001146 bupap-0.1.1/src/bupap/db/tables/user.py
+-rw-r--r--   0        0        0     2046 2023-06-05 17:43:31.022158 bupap-0.1.1/src/bupap/db/tables/work.py
+-rw-r--r--   0        0        0    23268 2023-06-09 10:47:15.829788 bupap-0.1.1/src/bupap/db/testdata.py
+-rw-r--r--   0        0        0      471 2023-06-11 09:02:32.917732 bupap-0.1.1/src/bupap/entrypoint/bupap_alembic.py
+-rw-r--r--   0        0        0      436 2023-06-11 09:02:32.921065 bupap-0.1.1/src/bupap/entrypoint/bupap_settings.py
+-rw-r--r--   0        0        0     3699 2023-06-11 10:37:36.184175 bupap-0.1.1/src/bupap/entrypoint/main.py
+-rw-r--r--   0        0        0      336 2023-06-09 10:19:05.314478 bupap-0.1.1/src/bupap/injection.py
+-rw-r--r--   0        0        0      882 2023-04-21 07:48:23.295613 bupap-0.1.1/src/bupap/log_config.py
+-rw-r--r--   0        0        0     2007 2023-05-03 16:20:37.159834 bupap-0.1.1/src/bupap/permissions.py
+-rw-r--r--   0        0        0      366 2023-06-18 09:22:32.018003 bupap-0.1.1/src/bupap/settings_default.toml
+-rw-r--r--   0        0        0        0 2023-04-18 18:45:59.268532 bupap-0.1.1/src/bupap/ui/__init__.py
+-rw-r--r--   0        0        0     1992 2023-06-09 10:19:05.517812 bupap-0.1.1/src/bupap/ui/common.py
+-rw-r--r--   0        0        0      473 2023-05-09 18:16:06.277872 bupap-0.1.1/src/bupap/ui/component/__init__.py
+-rw-r--r--   0        0        0     1970 2023-06-09 10:19:04.744480 bupap-0.1.1/src/bupap/ui/component/adduser.py
+-rw-r--r--   0        0        0      468 2023-06-09 10:19:04.644480 bupap-0.1.1/src/bupap/ui/component/avatar.py
+-rw-r--r--   0        0        0      596 2023-04-02 13:58:27.293968 bupap-0.1.1/src/bupap/ui/component/errors.js
+-rw-r--r--   0        0        0     3960 2023-06-11 09:02:33.014401 bupap-0.1.1/src/bupap/ui/component/errors.py
+-rw-r--r--   0        0        0     4702 2023-06-09 09:08:28.227746 bupap-0.1.1/src/bupap/ui/component/gantt.py
+-rw-r--r--   0        0        0    12377 2023-06-03 11:16:21.540333 bupap-0.1.1/src/bupap/ui/component/gantt.vue
+-rw-r--r--   0        0        0     1543 2023-06-09 10:19:04.471146 bupap-0.1.1/src/bupap/ui/component/header.py
+-rw-r--r--   0        0        0     1283 2023-05-15 17:22:30.300023 bupap-0.1.1/src/bupap/ui/component/pick_date.py
+-rw-r--r--   0        0        0     1300 2023-05-14 10:10:26.239776 bupap-0.1.1/src/bupap/ui/component/pick_date.vue
+-rw-r--r--   0        0        0      824 2023-03-31 17:20:09.472334 bupap-0.1.1/src/bupap/ui/component/router.js
+-rw-r--r--   0        0        0     5453 2023-06-09 10:19:04.354480 bupap-0.1.1/src/bupap/ui/component/router.py
+-rw-r--r--   0        0        0      624 2023-06-09 10:19:04.287814 bupap-0.1.1/src/bupap/ui/component/user_card.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:08:19.926227 bupap-0.1.1/src/bupap/ui/crud/__init__.py
+-rw-r--r--   0        0        0      759 2023-06-09 10:19:04.177814 bupap-0.1.1/src/bupap/ui/crud/common.py
+-rw-r--r--   0        0        0     3283 2023-06-09 10:19:04.057814 bupap-0.1.1/src/bupap/ui/crud/project.py
+-rw-r--r--   0        0        0    17461 2023-06-11 09:02:33.314408 bupap-0.1.1/src/bupap/ui/crud/task.py
+-rw-r--r--   0        0        0     4573 2023-06-09 10:19:03.964480 bupap-0.1.1/src/bupap/ui/crud/team.py
+-rw-r--r--   0        0        0     1069 2023-06-09 10:19:03.807814 bupap-0.1.1/src/bupap/ui/crud/user.py
+-rw-r--r--   0        0        0     4686 2023-06-09 10:19:03.774481 bupap-0.1.1/src/bupap/ui/crud/work.py
+-rw-r--r--   0        0        0      401 2023-05-01 11:06:05.700887 bupap-0.1.1/src/bupap/ui/page/__init__.py
+-rw-r--r--   0        0        0     1352 2023-06-09 11:51:57.867329 bupap-0.1.1/src/bupap/ui/page/index.py
+-rw-r--r--   0        0        0     1744 2023-06-09 11:52:02.273992 bupap-0.1.1/src/bupap/ui/page/login.py
+-rw-r--r--   0        0        0     4476 2023-06-09 11:52:13.130650 bupap-0.1.1/src/bupap/ui/page/projects.py
+-rw-r--r--   0        0        0    10847 2023-06-09 11:52:06.523988 bupap-0.1.1/src/bupap/ui/page/tasks.py
+-rw-r--r--   0        0        0    12154 2023-06-09 11:52:16.193981 bupap-0.1.1/src/bupap/ui/page/teams.py
+-rw-r--r--   0        0        0    16458 2023-06-09 11:52:19.503978 bupap-0.1.1/src/bupap/ui/page/users.py
+-rw-r--r--   0        0        0      265 2023-04-20 18:26:08.662931 bupap-0.1.1/src/bupap/ui/viewmodel/__init__.py
+-rw-r--r--   0        0        0      137 2023-04-21 07:48:23.412279 bupap-0.1.1/src/bupap/ui/viewmodel/login_information.py
+-rw-r--r--   0        0        0      258 2023-06-09 10:19:02.994482 bupap-0.1.1/src/bupap/ui/viewmodel/project.py
+-rw-r--r--   0        0        0      753 2023-06-09 10:19:02.974482 bupap-0.1.1/src/bupap/ui/viewmodel/task.py
+-rw-r--r--   0        0        0      155 2023-06-09 10:19:02.964482 bupap-0.1.1/src/bupap/ui/viewmodel/team.py
+-rw-r--r--   0        0        0      461 2023-06-09 10:19:02.961149 bupap-0.1.1/src/bupap/ui/viewmodel/user.py
+-rw-r--r--   0        0        0      975 2023-06-09 10:19:02.957816 bupap-0.1.1/src/bupap/ui/viewmodel/work.py
+-rw-r--r--   0        0        0     2040 1970-01-01 00:00:00.000000 bupap-0.1.1/PKG-INFO
```

### Comparing `bupap-0.1.0/LICENSE` & `bupap-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/pyproject.toml` & `bupap-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 [tool.poetry]
 name = "bupap"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["valgarf <valgarf@posteo.de>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/valgarf/bupap"
-include = ["README.md", "settings.toml"]
 exclude = ["src/bupap/data/EDITABLE_TAG"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 nicegui = "^1.2.17"
 sqlalchemy = "^2.0.16"
 bcrypt = "^4.0.1"
```

### Comparing `bupap-0.1.0/src/bupap/config.py` & `bupap-0.1.1/src/bupap/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,21 +14,23 @@
     ".secrets.toml",
 ]
 
 if not "BUPAP_ENV" in os.environ:
     os.environ["BUPAP_ENV"] = "testing"
     # TODO: remove me, makes 'testing' the default environment
 
+# os.environ["MERGE_ENABLED_FOR_DYNACONF"] = "1"
 settings = Dynaconf(
     envvar_prefix="BUPAP",
+    env_switcher="BUPAP_ENV",
+    merge_enable=True,
+    MERGE_ENABLED_FOR_DYNACONF=True,
     root_path=Path().resolve(),
     settings_files=settings_files,
     environments=True,
-    env_switcher="BUPAP_ENV",
-    merge_enable=True,
     validators=[
         Validator("initial_admin_password", default=None),
         Validator("editable", default=(Path(__file__).parent / "data" / "EDITABLE_TAG").exists()),
         Validator("pkg_root", default=str(Path(__file__).parent)),
         Validator("user_data_dir", default=user_data_dir("bupap")),
         Validator("cwd", default=str(Path().resolve())),
     ],
```

### Comparing `bupap-0.1.0/src/bupap/data/bupap_avatar.svg` & `bupap-0.1.1/src/bupap/data/bupap_avatar.svg`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/db/alembic/alembic.ini` & `bupap-0.1.1/src/bupap/db/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/db/alembic/env.py` & `bupap-0.1.1/src/bupap/db/alembic/env.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/db/alembic/versions/2023-04-28_initial.py` & `bupap-0.1.1/src/bupap/db/alembic/versions/2023-04-28_initial.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/db/database.py` & `bupap-0.1.1/src/bupap/db/database.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/db/defaults.py` & `bupap-0.1.1/src/bupap/db/defaults.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/db/tables/__init__.py` & `bupap-0.1.1/src/bupap/db/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/db/tables/base.py` & `bupap-0.1.1/src/bupap/db/tables/base.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/db/tables/estimate.py` & `bupap-0.1.1/src/bupap/db/tables/estimate.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/db/tables/history.py` & `bupap-0.1.1/src/bupap/db/tables/history.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/db/tables/project.py` & `bupap-0.1.1/src/bupap/db/tables/project.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/db/tables/role.py` & `bupap-0.1.1/src/bupap/db/tables/role.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/db/tables/schedule.py` & `bupap-0.1.1/src/bupap/db/tables/schedule.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/db/tables/task.py` & `bupap-0.1.1/src/bupap/db/tables/task.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/db/tables/team.py` & `bupap-0.1.1/src/bupap/db/tables/team.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/db/tables/user.py` & `bupap-0.1.1/src/bupap/db/tables/user.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/db/tables/work.py` & `bupap-0.1.1/src/bupap/db/tables/work.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/db/testdata.py` & `bupap-0.1.1/src/bupap/db/testdata.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/entrypoint/main.py` & `bupap-0.1.1/src/bupap/entrypoint/main.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/log_config.py` & `bupap-0.1.1/src/bupap/log_config.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/permissions.py` & `bupap-0.1.1/src/bupap/permissions.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/common.py` & `bupap-0.1.1/src/bupap/ui/common.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/component/adduser.py` & `bupap-0.1.1/src/bupap/ui/component/adduser.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/component/errors.js` & `bupap-0.1.1/src/bupap/ui/component/errors.js`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/component/errors.py` & `bupap-0.1.1/src/bupap/ui/component/errors.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/component/gantt.py` & `bupap-0.1.1/src/bupap/ui/component/gantt.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/component/gantt.vue` & `bupap-0.1.1/src/bupap/ui/component/gantt.vue`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/component/header.py` & `bupap-0.1.1/src/bupap/ui/component/header.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/component/pick_date.py` & `bupap-0.1.1/src/bupap/ui/component/pick_date.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/component/pick_date.vue` & `bupap-0.1.1/src/bupap/ui/component/pick_date.vue`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/component/router.js` & `bupap-0.1.1/src/bupap/ui/component/router.js`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/component/router.py` & `bupap-0.1.1/src/bupap/ui/component/router.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/component/user_card.py` & `bupap-0.1.1/src/bupap/ui/component/user_card.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/crud/common.py` & `bupap-0.1.1/src/bupap/ui/crud/common.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/crud/project.py` & `bupap-0.1.1/src/bupap/ui/crud/project.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/crud/task.py` & `bupap-0.1.1/src/bupap/ui/crud/task.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/crud/team.py` & `bupap-0.1.1/src/bupap/ui/crud/team.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/crud/user.py` & `bupap-0.1.1/src/bupap/ui/crud/user.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/crud/work.py` & `bupap-0.1.1/src/bupap/ui/crud/work.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/page/index.py` & `bupap-0.1.1/src/bupap/ui/page/index.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/page/login.py` & `bupap-0.1.1/src/bupap/ui/page/login.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/page/projects.py` & `bupap-0.1.1/src/bupap/ui/page/projects.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/page/tasks.py` & `bupap-0.1.1/src/bupap/ui/page/tasks.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/page/teams.py` & `bupap-0.1.1/src/bupap/ui/page/teams.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/page/users.py` & `bupap-0.1.1/src/bupap/ui/page/users.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/viewmodel/task.py` & `bupap-0.1.1/src/bupap/ui/viewmodel/task.py`

 * *Files identical despite different names*

### Comparing `bupap-0.1.0/src/bupap/ui/viewmodel/work.py` & `bupap-0.1.1/src/bupap/ui/viewmodel/work.py`

 * *Files identical despite different names*

