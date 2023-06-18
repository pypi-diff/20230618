# Comparing `tmp/celery-5.3.0rc2.tar.gz` & `tmp/celery-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celery-5.3.0rc2.tar", last modified: Wed May 31 14:55:48 2023, max compression
+gzip compressed data, was "celery-5.3.1.tar", last modified: Sun Jun 18 14:18:33 2023, max compression
```

## Comparing `celery-5.3.0rc2.tar` & `celery-5.3.1.tar`

### file list

```diff
@@ -1,749 +1,749 @@
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.539767 celery-5.3.0rc2/
--rw-rw-r--   0 asif      (1000) asif      (1000)     8184 2023-02-02 09:58:18.000000 celery-5.3.0rc2/CONTRIBUTORS.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)    24179 2023-05-31 14:38:43.000000 celery-5.3.0rc2/Changelog.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     2631 2021-10-12 14:26:47.000000 celery-5.3.0rc2/LICENSE
--rw-rw-r--   0 asif      (1000) asif      (1000)      709 2021-10-12 14:26:47.000000 celery-5.3.0rc2/MANIFEST.in
--rw-rw-r--   0 asif      (1000) asif      (1000)    17914 2023-05-31 14:55:48.539767 celery-5.3.0rc2/PKG-INFO
--rw-rw-r--   0 asif      (1000) asif      (1000)    15859 2023-05-31 14:43:46.000000 celery-5.3.0rc2/README.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)       84 2021-10-12 14:26:47.000000 celery-5.3.0rc2/TODO
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.443765 celery-5.3.0rc2/celery/
--rw-rw-r--   0 asif      (1000) asif      (1000)     5951 2023-05-31 14:42:37.000000 celery-5.3.0rc2/celery/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      409 2022-04-28 06:12:03.000000 celery-5.3.0rc2/celery/__main__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5029 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/_state.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.447766 celery-5.3.0rc2/celery/app/
--rw-rw-r--   0 asif      (1000) asif      (1000)     2430 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/app/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    23151 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/app/amqp.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1445 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/app/annotations.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2489 2022-06-29 10:52:39.000000 celery-5.3.0rc2/celery/app/autoretry.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2702 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/app/backends.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    50088 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/app/base.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6673 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/app/builtins.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    29170 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/app/control.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    15014 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/app/defaults.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1326 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/app/events.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9067 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/app/log.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2001 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/app/registry.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4527 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/app/routes.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    43264 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/app/task.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    28320 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/app/trace.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    13160 2022-07-28 12:22:51.000000 celery-5.3.0rc2/celery/app/utils.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.451766 celery-5.3.0rc2/celery/apps/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/apps/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5724 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/apps/beat.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    16360 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/apps/multi.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    13208 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/apps/worker.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.451766 celery-5.3.0rc2/celery/backends/
--rw-rw-r--   0 asif      (1000) asif      (1000)       23 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/backends/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7739 2022-06-29 10:52:39.000000 celery-5.3.0rc2/celery/backends/arangodb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    10309 2021-11-21 13:37:38.000000 celery-5.3.0rc2/celery/backends/asynchronous.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5127 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/backends/azureblockblob.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    43970 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/backends/base.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4817 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/backends/cache.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9006 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/backends/cassandra.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3816 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/backends/consul.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6777 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/backends/cosmosdbsql.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3393 2022-06-29 10:52:39.000000 celery-5.3.0rc2/celery/backends/couchbase.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2935 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/backends/couchdb.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.455766 celery-5.3.0rc2/celery/backends/database/
--rw-rw-r--   0 asif      (1000) asif      (1000)     7751 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/backends/database/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3351 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/backends/database/models.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3011 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/backends/database/session.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    17179 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/backends/dynamodb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8319 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/backends/elasticsearch.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3776 2022-06-29 10:52:39.000000 celery-5.3.0rc2/celery/backends/filesystem.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    10666 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/backends/mongodb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    26389 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/backends/redis.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    12077 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/backends/rpc.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2752 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/backends/s3.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    24338 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/beat.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.455766 celery-5.3.0rc2/celery/bin/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/bin/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    10023 2022-06-29 10:52:39.000000 celery-5.3.0rc2/celery/bin/amqp.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8525 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/bin/base.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2592 2022-07-28 12:22:51.000000 celery-5.3.0rc2/celery/bin/beat.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2370 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/bin/call.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7317 2023-05-31 06:35:39.000000 celery-5.3.0rc2/celery/bin/celery.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7058 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/bin/control.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2794 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/bin/events.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5796 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/bin/graph.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1058 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/bin/list.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4267 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/bin/logtool.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2108 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/bin/migrate.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    15364 2023-05-31 06:35:39.000000 celery-5.3.0rc2/celery/bin/multi.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2547 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/bin/purge.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      976 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/bin/result.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4778 2023-05-31 06:35:39.000000 celery-5.3.0rc2/celery/bin/shell.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3064 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/bin/upgrade.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    12884 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/bin/worker.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    12277 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/bootsteps.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    95874 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/canvas.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.455766 celery-5.3.0rc2/celery/concurrency/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1457 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/concurrency/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    51471 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/concurrency/asynpool.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4706 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/concurrency/base.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5126 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/concurrency/eventlet.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3387 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/concurrency/gevent.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5850 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/concurrency/prefork.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      754 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/concurrency/solo.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1920 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/concurrency/thread.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.455766 celery-5.3.0rc2/celery/contrib/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/contrib/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5003 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/contrib/abortable.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    14361 2022-04-28 06:12:03.000000 celery-5.3.0rc2/celery/contrib/migrate.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6754 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/contrib/pytest.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5005 2022-06-29 10:52:39.000000 celery-5.3.0rc2/celery/contrib/rdb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3391 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/contrib/sphinx.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.459766 celery-5.3.0rc2/celery/contrib/testing/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/contrib/testing/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3112 2022-06-29 10:52:39.000000 celery-5.3.0rc2/celery/contrib/testing/app.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7739 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/contrib/testing/manager.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4182 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/contrib/testing/mocks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      208 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/contrib/testing/tasks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5792 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/contrib/testing/worker.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.459766 celery-5.3.0rc2/celery/events/
--rw-rw-r--   0 asif      (1000) asif      (1000)      477 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/events/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    17961 2022-06-29 10:52:39.000000 celery-5.3.0rc2/celery/events/cursesmon.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8987 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/events/dispatcher.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3116 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/events/dumper.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1736 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/events/event.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4998 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/events/receiver.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3294 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/events/snapshot.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    25648 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/events/state.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9086 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/exceptions.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.459766 celery-5.3.0rc2/celery/fixups/
--rw-rw-r--   0 asif      (1000) asif      (1000)       14 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/fixups/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7161 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/fixups/django.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.459766 celery-5.3.0rc2/celery/loaders/
--rw-rw-r--   0 asif      (1000) asif      (1000)      490 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/loaders/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      199 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/loaders/app.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8825 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/loaders/base.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1520 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/loaders/default.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    16087 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/local.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    25290 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/platforms.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    35282 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/result.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    32003 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/schedules.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.459766 celery-5.3.0rc2/celery/security/
--rw-rw-r--   0 asif      (1000) asif      (1000)     2363 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/security/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4008 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/security/certificate.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1189 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/security/key.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4248 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/security/serialization.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      845 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/security/utils.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4384 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/signals.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3324 2022-04-28 06:12:03.000000 celery-5.3.0rc2/celery/states.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.463766 celery-5.3.0rc2/celery/utils/
--rw-rw-r--   0 asif      (1000) asif      (1000)      935 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2874 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/abstract.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    25427 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/utils/collections.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4709 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/debug.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3620 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/deprecated.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.463766 celery-5.3.0rc2/celery/utils/dispatch/
--rw-rw-r--   0 asif      (1000) asif      (1000)       74 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/dispatch/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    13603 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/dispatch/signal.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    12017 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/utils/functional.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9041 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/graph.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5032 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/utils/imports.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2871 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/utils/iso8601.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8757 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/utils/log.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2858 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/nodenames.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4215 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/objects.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8945 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/utils/saferepr.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8209 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/utils/serialization.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.463766 celery-5.3.0rc2/celery/utils/static/
--rw-rw-r--   0 asif      (1000) asif      (1000)      299 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/static/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2556 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/static/celery_128.png
--rw-rw-r--   0 asif      (1000) asif      (1000)     1085 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/sysinfo.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4532 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/utils/term.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5844 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/utils/text.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9552 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/utils/threads.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    14987 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/utils/time.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4813 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/utils/timer2.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.467766 celery-5.3.0rc2/celery/worker/
--rw-rw-r--   0 asif      (1000) asif      (1000)       95 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4593 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/autoscale.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7497 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/worker/components.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.467766 celery-5.3.0rc2/celery/worker/consumer/
--rw-rw-r--   0 asif      (1000) asif      (1000)      391 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/consumer/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      525 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/consumer/agent.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1026 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/consumer/connection.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    28320 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/worker/consumer/consumer.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      946 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/consumer/control.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2054 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/consumer/events.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6833 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/consumer/gossip.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      930 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/consumer/heart.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2519 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/consumer/mingle.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1960 2022-03-18 11:40:50.000000 celery-5.3.0rc2/celery/worker/consumer/tasks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    19884 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/worker/control.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2107 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/heartbeat.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4433 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/loops.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3630 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/pidbox.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    27229 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/worker/request.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8583 2023-05-31 06:35:53.000000 celery-5.3.0rc2/celery/worker/state.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7349 2021-10-12 14:26:47.000000 celery-5.3.0rc2/celery/worker/strategy.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    14460 2023-02-02 09:58:18.000000 celery-5.3.0rc2/celery/worker/worker.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.443765 celery-5.3.0rc2/celery.egg-info/
--rw-rw-r--   0 asif      (1000) asif      (1000)    17914 2023-05-31 14:55:47.000000 celery-5.3.0rc2/celery.egg-info/PKG-INFO
--rw-rw-r--   0 asif      (1000) asif      (1000)    21130 2023-05-31 14:55:48.000000 celery-5.3.0rc2/celery.egg-info/SOURCES.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)        1 2023-05-31 14:55:47.000000 celery-5.3.0rc2/celery.egg-info/dependency_links.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       49 2023-05-31 14:55:47.000000 celery-5.3.0rc2/celery.egg-info/entry_points.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)     1623 2023-05-31 14:55:47.000000 celery-5.3.0rc2/celery.egg-info/requires.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)        7 2023-05-31 14:55:47.000000 celery-5.3.0rc2/celery.egg-info/top_level.txt
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.471766 celery-5.3.0rc2/docs/
--rw-rw-r--   0 asif      (1000) asif      (1000)     5293 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/AUTHORS.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)     8111 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/Makefile
--rw-rw-r--   0 asif      (1000) asif      (1000)      494 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/THANKS
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.471766 celery-5.3.0rc2/docs/_ext/
--rw-rw-r--   0 asif      (1000) asif      (1000)     5164 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/_ext/celerydocs.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.471766 celery-5.3.0rc2/docs/_static/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/_static/.keep
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.471766 celery-5.3.0rc2/docs/_templates/
--rw-rw-r--   0 asif      (1000) asif      (1000)      486 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/_templates/sidebardonations.html
--rw-rw-r--   0 asif      (1000) asif      (1000)       30 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/changelog.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      981 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/community.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     2597 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/conf.py
--rw-rw-r--   0 asif      (1000) asif      (1000)       83 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/configuration.html
--rw-rw-r--   0 asif      (1000) asif      (1000)       33 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/contributing.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      931 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/copyright.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.471766 celery-5.3.0rc2/docs/django/
--rw-rw-r--   0 asif      (1000) asif      (1000)     7886 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/django/first-steps-with-django.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      137 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/django/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    29852 2023-05-31 06:35:53.000000 celery-5.3.0rc2/docs/faq.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.471766 celery-5.3.0rc2/docs/getting-started/
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.471766 celery-5.3.0rc2/docs/getting-started/backends-and-brokers/
--rw-rw-r--   0 asif      (1000) asif      (1000)     3903 2023-05-31 06:35:53.000000 celery-5.3.0rc2/docs/getting-started/backends-and-brokers/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     5010 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/getting-started/backends-and-brokers/rabbitmq.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     7239 2023-05-31 06:35:53.000000 celery-5.3.0rc2/docs/getting-started/backends-and-brokers/redis.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    10843 2022-03-18 11:40:50.000000 celery-5.3.0rc2/docs/getting-started/backends-and-brokers/sqs.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    14995 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/getting-started/first-steps-with-celery.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      226 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/getting-started/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    10903 2021-12-29 05:20:59.000000 celery-5.3.0rc2/docs/getting-started/introduction.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    22787 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/getting-started/next-steps.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      132 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/getting-started/resources.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     4448 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/glossary.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.475766 celery-5.3.0rc2/docs/history/
--rw-rw-r--   0 asif      (1000) asif      (1000)    58104 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/history/changelog-1.0.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    34009 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/history/changelog-2.0.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    23550 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/changelog-2.1.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    33558 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/history/changelog-2.2.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    11200 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/history/changelog-2.3.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    13012 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/history/changelog-2.4.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     5414 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/changelog-2.5.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    49344 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/history/changelog-3.0.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    52336 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/history/changelog-3.1.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     6432 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/changelog-4.0.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     8950 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/changelog-4.1.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    13593 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/changelog-4.2.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    17251 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/changelog-4.3.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    24332 2021-11-21 13:37:38.000000 celery-5.3.0rc2/docs/history/changelog-4.4.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     5720 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/history/changelog-5.0.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     5592 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/history/changelog-5.1.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      675 2021-11-21 13:37:38.000000 celery-5.3.0rc2/docs/history/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    16026 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/whatsnew-2.5.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    30892 2021-11-21 13:37:38.000000 celery-5.3.0rc2/docs/history/whatsnew-3.0.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    44129 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/whatsnew-3.1.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    76466 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/history/whatsnew-4.0.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     8244 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/whatsnew-4.1.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    35711 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/whatsnew-4.2.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    16865 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/whatsnew-4.3.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     6999 2021-11-21 13:37:38.000000 celery-5.3.0rc2/docs/history/whatsnew-4.4.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    10957 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/history/whatsnew-5.0.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    14128 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/history/whatsnew-5.1.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.479766 celery-5.3.0rc2/docs/images/
--rw-rw-r--   0 asif      (1000) asif      (1000)    14168 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/images/celery-banner-small.png
--rw-rw-r--   0 asif      (1000) asif      (1000)    14038 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/images/celery-banner.png
--rw-rw-r--   0 asif      (1000) asif      (1000)     2556 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/images/celery_128.png
--rw-rw-r--   0 asif      (1000) asif      (1000)     8658 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/images/celery_512.png
--rw-rw-r--   0 asif      (1000) asif      (1000)    77397 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/images/celeryevshotsm.jpg
--rw-rw-r--   0 asif      (1000) asif      (1000)    88879 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/images/dashboard.png
--rw-rw-r--   0 asif      (1000) asif      (1000)     4286 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/images/favicon.ico
--rw-rw-r--   0 asif      (1000) asif      (1000)   146412 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/images/monitor.png
--rw-rw-r--   0 asif      (1000) asif      (1000)    35894 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/images/result_graph.png
--rw-rw-r--   0 asif      (1000) asif      (1000)    99783 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/images/worker_graph_full.png
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.479766 celery-5.3.0rc2/docs/includes/
--rw-rw-r--   0 asif      (1000) asif      (1000)     4023 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/includes/installation.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)     6422 2023-05-31 14:43:08.000000 celery-5.3.0rc2/docs/includes/introduction.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)     1375 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/includes/resources.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)     1613 2021-11-21 13:37:38.000000 celery-5.3.0rc2/docs/index.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.479766 celery-5.3.0rc2/docs/internals/
--rw-rw-r--   0 asif      (1000) asif      (1000)     5985 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/app-overview.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     5696 2022-04-28 06:12:03.000000 celery-5.3.0rc2/docs/internals/deprecation.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     8586 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/guide.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      206 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     9898 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/protocol.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.487766 celery-5.3.0rc2/docs/internals/reference/
--rw-rw-r--   0 asif      (1000) asif      (1000)      226 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery._state.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      257 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.app.annotations.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      224 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.app.routes.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      239 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.app.trace.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.arangodb.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.asynchronous.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      293 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.azureblockblob.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      243 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.base.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      256 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.cache.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      278 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.cassandra.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      253 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.consul.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      284 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.cosmosdbsql.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      270 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.couchbase.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      262 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.couchdb.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      276 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.database.models.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      293 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.database.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      283 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.database.session.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      265 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.dynamodb.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      280 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.elasticsearch.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      269 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.filesystem.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      264 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.mongodb.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      254 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.redis.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      242 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.rpc.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      206 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      245 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.backends.s3.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      270 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.concurrency.base.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      310 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.concurrency.eventlet.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      304 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.concurrency.gevent.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      307 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.concurrency.prefork.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      229 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.concurrency.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      310 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.concurrency.solo.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      304 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.concurrency.thread.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      260 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.events.cursesmon.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      251 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.events.dumper.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      257 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.events.snapshot.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      231 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.platforms.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      272 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.security.certificate.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      248 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.security.key.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      278 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.security.serialization.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      254 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.security.utils.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      256 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.abstract.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      252 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.collections.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      260 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.deprecated.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      252 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.dispatch.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      295 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.dispatch.signal.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      282 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.functional.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      245 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.graph.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      273 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.imports.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.iso8601.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      261 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.log.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      257 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.nodenames.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.objects.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      195 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      256 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.saferepr.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      273 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.serialization.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.sysinfo.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      264 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.term.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      264 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.text.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      251 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.threads.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      258 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.time.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      224 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.utils.timer2.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      256 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.worker.autoscale.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      259 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.worker.components.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      260 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.worker.control.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      266 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.worker.heartbeat.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      236 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.worker.loops.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      239 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/celery.worker.pidbox.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     1960 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/reference/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     1452 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/internals/worker.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     7675 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/make.bat
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.499766 celery-5.3.0rc2/docs/reference/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1379 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.amqp.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      237 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.autoretry.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      234 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.backends.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      268 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.builtins.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      265 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.control.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      290 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.defaults.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      222 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.events.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      213 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.log.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      228 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.registry.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      288 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      226 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.task.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      219 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.app.utils.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      253 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.apps.beat.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      236 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.apps.multi.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      239 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.apps.worker.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      220 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.beat.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      189 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/reference/celery.bin.amqp.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      216 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.base.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      254 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.beat.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      258 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.call.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      242 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.celery.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.control.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      264 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.events.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      261 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.graph.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      258 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.list.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.logtool.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.migrate.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      249 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.multi.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      261 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.purge.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      264 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.result.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      261 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.shell.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.upgrade.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      242 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bin.worker.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      239 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.bootsteps.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      290 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.contrib.abortable.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      230 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.contrib.migrate.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      273 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.contrib.pytest.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      256 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.contrib.rdb.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      184 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.contrib.sphinx.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      288 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.contrib.testing.app.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      300 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.contrib.testing.manager.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.contrib.testing.mocks.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      297 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.contrib.testing.worker.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      304 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.events.dispatcher.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.events.event.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      303 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.events.receiver.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      194 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.events.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.events.state.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      222 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.exceptions.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      227 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.loaders.app.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      250 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.loaders.base.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      255 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.loaders.default.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      237 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.loaders.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      204 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.result.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     3497 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      261 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.schedules.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      200 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.security.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      257 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.signals.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      106 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.states.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      871 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.utils.debug.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      291 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.consumer.agent.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      306 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.consumer.connection.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      300 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.consumer.consumer.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      297 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.consumer.control.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.consumer.events.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.consumer.gossip.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      291 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.consumer.heart.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.consumer.mingle.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      273 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.consumer.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      291 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.consumer.tasks.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      244 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.request.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      226 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      236 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.state.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      245 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.strategy.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      239 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/celery.worker.worker.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      143 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/cli.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     1952 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/reference/index.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.499766 celery-5.3.0rc2/docs/sec/
--rw-rw-r--   0 asif      (1000) asif      (1000)     2921 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/sec/CELERYSA-0001.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)     2656 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/sec/CELERYSA-0002.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)     1551 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/sec/CELERYSA-0003.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)     4879 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/spelling_wordlist.txt
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.499766 celery-5.3.0rc2/docs/templates/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1186 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/templates/readme.txt
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.499766 celery-5.3.0rc2/docs/tutorials/
--rw-rw-r--   0 asif      (1000) asif      (1000)       86 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/tutorials/daemonizing.html
--rw-rw-r--   0 asif      (1000) asif      (1000)       91 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/tutorials/debugging.html
--rw-rw-r--   0 asif      (1000) asif      (1000)      121 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/tutorials/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     2766 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/tutorials/task-cookbook.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.503766 celery-5.3.0rc2/docs/userguide/
--rw-rw-r--   0 asif      (1000) asif      (1000)    14779 2022-04-28 06:12:03.000000 celery-5.3.0rc2/docs/userguide/application.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    25233 2023-05-31 06:35:53.000000 celery-5.3.0rc2/docs/userguide/calling.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    38007 2023-05-31 06:35:53.000000 celery-5.3.0rc2/docs/userguide/canvas.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.503766 celery-5.3.0rc2/docs/userguide/concurrency/
--rw-rw-r--   0 asif      (1000) asif      (1000)     2665 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/userguide/concurrency/eventlet.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      140 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/userguide/concurrency/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    98436 2023-05-31 06:35:53.000000 celery-5.3.0rc2/docs/userguide/configuration.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    17699 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/userguide/daemonizing.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     3131 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/userguide/debugging.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    30057 2022-03-18 11:40:50.000000 celery-5.3.0rc2/docs/userguide/extending.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      372 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/userguide/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    21759 2023-05-31 06:35:53.000000 celery-5.3.0rc2/docs/userguide/monitoring.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     8437 2021-12-29 05:20:59.000000 celery-5.3.0rc2/docs/userguide/optimizing.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    20950 2023-05-31 06:35:53.000000 celery-5.3.0rc2/docs/userguide/periodic-tasks.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    24323 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/userguide/routing.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     8693 2022-07-28 12:22:51.000000 celery-5.3.0rc2/docs/userguide/security.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    18113 2023-05-31 06:35:53.000000 celery-5.3.0rc2/docs/userguide/signals.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      345 2021-10-12 14:26:47.000000 celery-5.3.0rc2/docs/userguide/sphinx.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    64543 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/userguide/tasks.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    11146 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/userguide/testing.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    34758 2023-02-02 09:58:18.000000 celery-5.3.0rc2/docs/userguide/workers.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    12812 2022-08-01 10:53:57.000000 celery-5.3.0rc2/docs/whatsnew-5.2.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.503766 celery-5.3.0rc2/examples/
--rw-rw-r--   0 asif      (1000) asif      (1000)      303 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/README.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.503766 celery-5.3.0rc2/examples/app/
--rw-rw-r--   0 asif      (1000) asif      (1000)      822 2022-06-29 10:52:39.000000 celery-5.3.0rc2/examples/app/myapp.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.503766 celery-5.3.0rc2/examples/celery_http_gateway/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1382 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/celery_http_gateway/README.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/celery_http_gateway/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      385 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/celery_http_gateway/manage.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3001 2021-11-21 13:37:38.000000 celery-5.3.0rc2/examples/celery_http_gateway/settings.py
--rw-rw-r--   0 asif      (1000) asif      (1000)       88 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/celery_http_gateway/tasks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      678 2022-03-18 11:40:50.000000 celery-5.3.0rc2/examples/celery_http_gateway/urls.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.503766 celery-5.3.0rc2/examples/django/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1546 2022-08-01 10:53:57.000000 celery-5.3.0rc2/examples/django/README.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.503766 celery-5.3.0rc2/examples/django/demoapp/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/django/demoapp/__init__.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.503766 celery-5.3.0rc2/examples/django/demoapp/migrations/
--rw-rw-r--   0 asif      (1000) asif      (1000)      486 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/django/demoapp/migrations/0001_initial.py
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/django/demoapp/migrations/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      103 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/django/demoapp/models.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      437 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/django/demoapp/tasks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)       26 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/django/demoapp/views.py
--rwxrwxr-x   0 asif      (1000) asif      (1000)      248 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/django/manage.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/examples/django/proj/
--rw-rw-r--   0 asif      (1000) asif      (1000)      174 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/django/proj/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      659 2022-06-29 10:52:39.000000 celery-5.3.0rc2/examples/django/proj/celery.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3639 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/django/proj/settings.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      556 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/django/proj/urls.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1132 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/django/proj/wsgi.py
--rw-rw-r--   0 asif      (1000) asif      (1000)       47 2023-02-02 09:58:18.000000 celery-5.3.0rc2/examples/django/requirements.txt
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/examples/eventlet/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1449 2022-04-28 06:12:03.000000 celery-5.3.0rc2/examples/eventlet/README.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     1673 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/eventlet/bulk_task_producer.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      312 2022-04-28 06:12:03.000000 celery-5.3.0rc2/examples/eventlet/celeryconfig.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      306 2022-04-28 06:12:03.000000 celery-5.3.0rc2/examples/eventlet/tasks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2009 2022-04-28 06:12:03.000000 celery-5.3.0rc2/examples/eventlet/webcrawler.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/examples/gevent/
--rw-rw-r--   0 asif      (1000) asif      (1000)      255 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/gevent/celeryconfig.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      325 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/gevent/tasks.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/examples/next-steps/
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/examples/next-steps/proj/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/next-steps/proj/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/next-steps/proj/celery.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      167 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/next-steps/proj/tasks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1224 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/next-steps/setup.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/examples/periodic-tasks/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1518 2022-08-01 10:53:57.000000 celery-5.3.0rc2/examples/periodic-tasks/myapp.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/examples/resultgraph/
--rw-rw-r--   0 asif      (1000) asif      (1000)     2860 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/resultgraph/tasks.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/examples/security/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1058 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/security/mysecureapp.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/examples/security/ssl/
--rw-rw-r--   0 asif      (1000) asif      (1000)     3243 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/security/ssl/worker.key
--rw-rw-r--   0 asif      (1000) asif      (1000)     1923 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/security/ssl/worker.pem
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/examples/stamping/
--rw-rw-r--   0 asif      (1000) asif      (1000)      103 2023-02-02 09:58:18.000000 celery-5.3.0rc2/examples/stamping/config.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1358 2023-05-31 06:35:53.000000 celery-5.3.0rc2/examples/stamping/examples.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1806 2023-05-31 06:35:53.000000 celery-5.3.0rc2/examples/stamping/myapp.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2548 2023-05-31 06:35:53.000000 celery-5.3.0rc2/examples/stamping/revoke_example.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3311 2023-05-31 06:35:53.000000 celery-5.3.0rc2/examples/stamping/tasks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2410 2023-05-31 06:35:53.000000 celery-5.3.0rc2/examples/stamping/visitors.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/examples/tutorial/
--rw-rw-r--   0 asif      (1000) asif      (1000)      158 2021-10-12 14:26:47.000000 celery-5.3.0rc2/examples/tutorial/tasks.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.439766 celery-5.3.0rc2/extra/
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/extra/bash-completion/
--rw-rw-r--   0 asif      (1000) asif      (1000)      636 2021-10-12 14:26:47.000000 celery-5.3.0rc2/extra/bash-completion/celery.bash
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/extra/generic-init.d/
--rwxrwxr-x   0 asif      (1000) asif      (1000)     9068 2022-08-01 10:53:57.000000 celery-5.3.0rc2/extra/generic-init.d/celerybeat
--rwxrwxr-x   0 asif      (1000) asif      (1000)    10813 2023-05-31 06:35:53.000000 celery-5.3.0rc2/extra/generic-init.d/celeryd
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.507767 celery-5.3.0rc2/extra/macOS/
--rw-rw-r--   0 asif      (1000) asif      (1000)      751 2021-10-12 14:26:47.000000 celery-5.3.0rc2/extra/macOS/org.celeryq.beat.plist
--rw-rw-r--   0 asif      (1000) asif      (1000)      757 2021-10-12 14:26:47.000000 celery-5.3.0rc2/extra/macOS/org.celeryq.worker.plist
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.511767 celery-5.3.0rc2/extra/supervisord/
--rw-rw-r--   0 asif      (1000) asif      (1000)      134 2021-10-12 14:26:47.000000 celery-5.3.0rc2/extra/supervisord/celery.sh
--rw-rw-r--   0 asif      (1000) asif      (1000)      699 2021-10-12 14:26:47.000000 celery-5.3.0rc2/extra/supervisord/celerybeat.conf
--rw-rw-r--   0 asif      (1000) asif      (1000)      949 2021-10-12 14:26:47.000000 celery-5.3.0rc2/extra/supervisord/celeryd.conf
--rw-rw-r--   0 asif      (1000) asif      (1000)      982 2023-02-02 09:58:18.000000 celery-5.3.0rc2/extra/supervisord/supervisord.conf
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.511767 celery-5.3.0rc2/extra/systemd/
--rw-rw-r--   0 asif      (1000) asif      (1000)      506 2022-08-01 10:53:57.000000 celery-5.3.0rc2/extra/systemd/celery.conf
--rw-rw-r--   0 asif      (1000) asif      (1000)      740 2021-10-12 14:26:47.000000 celery-5.3.0rc2/extra/systemd/celery.service
--rw-rw-r--   0 asif      (1000) asif      (1000)       78 2021-10-12 14:26:47.000000 celery-5.3.0rc2/extra/systemd/celery.tmpfiles
--rw-rw-r--   0 asif      (1000) asif      (1000)      395 2021-10-12 14:26:47.000000 celery-5.3.0rc2/extra/systemd/celerybeat.service
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.511767 celery-5.3.0rc2/extra/zsh-completion/
--rw-rw-r--   0 asif      (1000) asif      (1000)     6244 2021-10-12 14:26:47.000000 celery-5.3.0rc2/extra/zsh-completion/celery.zsh
--rw-rw-r--   0 asif      (1000) asif      (1000)     1216 2023-05-31 06:35:53.000000 celery-5.3.0rc2/pyproject.toml
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.511767 celery-5.3.0rc2/requirements/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1454 2023-02-02 09:58:18.000000 celery-5.3.0rc2/requirements/README.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      276 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/default.txt
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.511767 celery-5.3.0rc2/requirements/deps/
--rw-rw-r--   0 asif      (1000) asif      (1000)       10 2021-10-12 14:26:47.000000 celery-5.3.0rc2/requirements/deps/mock.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      151 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/dev.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      187 2023-02-02 09:58:18.000000 celery-5.3.0rc2/requirements/docs.txt
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.515767 celery-5.3.0rc2/requirements/extras/
--rw-rw-r--   0 asif      (1000) asif      (1000)       16 2022-06-29 10:52:39.000000 celery-5.3.0rc2/requirements/extras/arangodb.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       21 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/extras/auth.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       28 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/extras/azureblockblob.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      111 2021-10-12 14:26:47.000000 celery-5.3.0rc2/requirements/extras/brotli.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       28 2022-06-29 10:52:39.000000 celery-5.3.0rc2/requirements/extras/cassandra.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       22 2022-06-29 10:52:39.000000 celery-5.3.0rc2/requirements/extras/consul.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       20 2022-04-28 06:12:03.000000 celery-5.3.0rc2/requirements/extras/cosmosdbsql.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      119 2021-12-29 05:20:59.000000 celery-5.3.0rc2/requirements/extras/couchbase.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       18 2022-06-29 10:52:39.000000 celery-5.3.0rc2/requirements/extras/couchdb.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       15 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/extras/django.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       14 2022-06-29 10:52:39.000000 celery-5.3.0rc2/requirements/extras/dynamodb.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       18 2022-03-18 11:40:50.000000 celery-5.3.0rc2/requirements/extras/elasticsearch.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       40 2021-11-21 13:37:38.000000 celery-5.3.0rc2/requirements/extras/eventlet.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       14 2021-11-21 13:37:38.000000 celery-5.3.0rc2/requirements/extras/gevent.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       19 2021-10-12 14:26:47.000000 celery-5.3.0rc2/requirements/extras/librabbitmq.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       45 2023-02-02 09:58:18.000000 celery-5.3.0rc2/requirements/extras/memcache.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       20 2022-04-28 06:12:03.000000 celery-5.3.0rc2/requirements/extras/mongodb.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       15 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/extras/msgpack.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       23 2022-04-28 06:12:03.000000 celery-5.3.0rc2/requirements/extras/pymemcache.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)        6 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/extras/pyro.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       21 2022-06-29 10:52:39.000000 celery-5.3.0rc2/requirements/extras/pytest.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       13 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/extras/redis.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       16 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/extras/s3.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       27 2021-10-12 14:26:47.000000 celery-5.3.0rc2/requirements/extras/slmq.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       53 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/extras/solar.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       27 2021-10-12 14:26:47.000000 celery-5.3.0rc2/requirements/extras/sphinxautobuild.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       24 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/extras/sqlalchemy.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       21 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/extras/sqs.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       73 2021-10-12 14:26:47.000000 celery-5.3.0rc2/requirements/extras/tblib.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       39 2021-10-12 14:26:47.000000 celery-5.3.0rc2/requirements/extras/thread.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       13 2021-10-12 14:26:47.000000 celery-5.3.0rc2/requirements/extras/yaml.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       14 2023-02-02 09:58:18.000000 celery-5.3.0rc2/requirements/extras/zeromq.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       13 2021-10-12 14:26:47.000000 celery-5.3.0rc2/requirements/extras/zookeeper.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       18 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/extras/zstd.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      212 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/pkgutils.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       19 2021-10-12 14:26:47.000000 celery-5.3.0rc2/requirements/security.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      175 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/test-ci-base.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      539 2022-06-29 10:52:39.000000 celery-5.3.0rc2/requirements/test-ci-default.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      160 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/test-integration.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       17 2021-10-12 14:26:47.000000 celery-5.3.0rc2/requirements/test-pypy3.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      307 2023-05-31 06:35:53.000000 celery-5.3.0rc2/requirements/test.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      485 2023-05-31 14:55:48.539767 celery-5.3.0rc2/setup.cfg
--rwxrwxr-x   0 asif      (1000) asif      (1000)     4509 2023-05-31 06:54:18.000000 celery-5.3.0rc2/setup.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.515767 celery-5.3.0rc2/t/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/__init__.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.515767 celery-5.3.0rc2/t/benchmarks/
--rw-rw-r--   0 asif      (1000) asif      (1000)     2816 2022-06-29 10:52:39.000000 celery-5.3.0rc2/t/benchmarks/bench_worker.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.519767 celery-5.3.0rc2/t/integration/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/integration/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2350 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/integration/conftest.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    12427 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/integration/tasks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1120 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/integration/test_backend.py
--rw-rw-r--   0 asif      (1000) asif      (1000)   132248 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/integration/test_canvas.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7796 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/integration/test_inspect.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3459 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/integration/test_security.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    18656 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/integration/test_tasks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      688 2022-06-29 10:52:39.000000 celery-5.3.0rc2/t/integration/test_worker.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      293 2022-06-29 10:52:39.000000 celery-5.3.0rc2/t/integration/test_worker_config.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      226 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/skip.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.519767 celery-5.3.0rc2/t/unit/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/__init__.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.519767 celery-5.3.0rc2/t/unit/app/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/app/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    13768 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/app/test_amqp.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1338 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/app/test_annotations.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    41390 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/app/test_app.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4542 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/app/test_backends.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    29065 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/app/test_beat.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5528 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/app/test_builtins.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      356 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/app/test_celery.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    19105 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/app/test_control.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1608 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/app/test_defaults.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      801 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/app/test_exceptions.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8823 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/app/test_loaders.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    11820 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/app/test_log.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2349 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/app/test_registry.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8026 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/app/test_routes.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    37835 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/app/test_schedules.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1790 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/app/test_utils.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.519767 celery-5.3.0rc2/t/unit/apps/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/apps/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    16234 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/apps/test_multi.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.523767 celery-5.3.0rc2/t/unit/backends/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/backends/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4362 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_arangodb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6874 2021-11-21 13:37:38.000000 celery-5.3.0rc2/t/unit/backends/test_asynchronous.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6794 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_azureblockblob.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    45945 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/backends/test_base.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    10318 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_cache.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8669 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_cassandra.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1448 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_consul.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4994 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_cosmosdbsql.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4846 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_couchbase.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3971 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_couchdb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    15087 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/backends/test_database.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    19214 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_dynamodb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    32601 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_elasticsearch.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4435 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_filesystem.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    28352 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/backends/test_mongodb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    50595 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_redis.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3692 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/backends/test_rpc.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6654 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/backends/test_s3.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.523767 celery-5.3.0rc2/t/unit/bin/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/bin/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)       18 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/bin/celery.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.523767 celery-5.3.0rc2/t/unit/bin/proj/
--rw-rw-r--   0 asif      (1000) asif      (1000)       64 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/bin/proj/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      121 2022-06-29 10:52:39.000000 celery-5.3.0rc2/t/unit/bin/proj/app.py
--rw-rw-r--   0 asif      (1000) asif      (1000)       22 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/bin/proj/app2.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      109 2022-07-28 12:22:51.000000 celery-5.3.0rc2/t/unit/bin/proj/scheduler.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1116 2022-07-28 12:22:51.000000 celery-5.3.0rc2/t/unit/bin/test_beat.py
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/bin/test_multi.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      529 2022-06-29 10:52:39.000000 celery-5.3.0rc2/t/unit/bin/test_worker.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.523767 celery-5.3.0rc2/t/unit/concurrency/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/concurrency/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5687 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/concurrency/test_concurrency.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4721 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/concurrency/test_eventlet.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3146 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/concurrency/test_gevent.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1837 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/concurrency/test_pool.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    16398 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/concurrency/test_prefork.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      848 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/concurrency/test_solo.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      728 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/concurrency/test_thread.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    23214 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/conftest.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.527767 celery-5.3.0rc2/t/unit/contrib/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/contrib/__init__.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.527767 celery-5.3.0rc2/t/unit/contrib/proj/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/contrib/proj/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      183 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/contrib/proj/conf.py
--rw-rw-r--   0 asif      (1000) asif      (1000)       93 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/contrib/proj/contents.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      249 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/contrib/proj/foo.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      113 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/contrib/proj/xyzzy.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1394 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/contrib/test_abortable.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    10615 2022-03-18 11:40:50.000000 celery-5.3.0rc2/t/unit/contrib/test_migrate.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      785 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/contrib/test_pytest.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3146 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/contrib/test_rdb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      731 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/contrib/test_sphinx.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1474 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/contrib/test_worker.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.527767 celery-5.3.0rc2/t/unit/events/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/events/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2304 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/events/test_cursesmon.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    11372 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/events/test_events.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3359 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/events/test_snapshot.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    22261 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/events/test_state.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.527767 celery-5.3.0rc2/t/unit/fixups/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/fixups/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    11013 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/fixups/test_django.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.531767 celery-5.3.0rc2/t/unit/security/
--rw-rw-r--   0 asif      (1000) asif      (1000)     7344 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/security/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      109 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/security/case.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3333 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/security/test_certificate.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1570 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/security/test_key.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6219 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/security/test_security.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2224 2022-03-18 11:40:50.000000 celery-5.3.0rc2/t/unit/security/test_serialization.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.531767 celery-5.3.0rc2/t/unit/tasks/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/tasks/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    68472 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/tasks/test_canvas.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    12308 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/tasks/test_chord.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3134 2022-06-29 10:52:39.000000 celery-5.3.0rc2/t/unit/tasks/test_context.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    34984 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/tasks/test_result.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    52722 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/tasks/test_stamping.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1085 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/tasks/test_states.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    56857 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/tasks/test_tasks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    21991 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/tasks/test_trace.py
--rw-rw-r--   0 asif      (1000) asif      (1000)       78 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/tasks/unit_tasks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      989 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/test_canvas.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.535767 celery-5.3.0rc2/t/unit/utils/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    12855 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/utils/test_collections.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2357 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/test_debug.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1739 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/utils/test_deprecated.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5233 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/test_dispatcher.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    13576 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/utils/test_functional.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1935 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/test_graph.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3272 2022-03-18 11:40:50.000000 celery-5.3.0rc2/t/unit/utils/test_imports.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8515 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/utils/test_local.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      202 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/test_nodenames.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      172 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/test_objects.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1386 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/test_pickle.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    32949 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/utils/test_platforms.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5555 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/test_saferepr.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3219 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/utils/test_serialization.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      751 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/test_sysinfo.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1734 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/test_term.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1935 2022-03-18 11:40:50.000000 celery-5.3.0rc2/t/unit/utils/test_text.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2427 2022-03-18 11:40:50.000000 celery-5.3.0rc2/t/unit/utils/test_threads.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    11465 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/utils/test_time.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3215 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/test_timer2.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      624 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/utils/test_utils.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-05-31 14:55:48.539767 celery-5.3.0rc2/t/unit/worker/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/worker/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7574 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/worker/test_autoscale.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9415 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/worker/test_bootsteps.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2461 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/worker/test_components.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    30428 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/worker/test_consumer.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    28334 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/worker/test_control.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2384 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/worker/test_heartbeat.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    18256 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/worker/test_loops.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    48131 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/worker/test_request.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      238 2021-10-12 14:26:47.000000 celery-5.3.0rc2/t/unit/worker/test_revoke.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6339 2023-05-31 06:35:53.000000 celery-5.3.0rc2/t/unit/worker/test_state.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    10989 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/worker/test_strategy.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    39912 2023-02-02 09:58:18.000000 celery-5.3.0rc2/t/unit/worker/test_worker.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.758499 celery-5.3.1/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8184 2023-02-02 09:58:18.000000 celery-5.3.1/CONTRIBUTORS.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)    25016 2023-06-18 14:11:03.000000 celery-5.3.1/Changelog.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2717 2023-06-18 13:56:43.000000 celery-5.3.1/LICENSE
+-rw-rw-r--   0 asif      (1000) asif      (1000)      709 2021-10-12 14:26:47.000000 celery-5.3.1/MANIFEST.in
+-rw-rw-r--   0 asif      (1000) asif      (1000)    18020 2023-06-18 14:18:33.758499 celery-5.3.1/PKG-INFO
+-rw-rw-r--   0 asif      (1000) asif      (1000)    15917 2023-06-18 14:16:05.000000 celery-5.3.1/README.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)       84 2021-10-12 14:26:47.000000 celery-5.3.1/TODO
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.666497 celery-5.3.1/celery/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5949 2023-06-18 14:11:51.000000 celery-5.3.1/celery/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      409 2022-04-28 06:12:03.000000 celery-5.3.1/celery/__main__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5029 2021-10-12 14:26:47.000000 celery-5.3.1/celery/_state.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.670497 celery-5.3.1/celery/app/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2430 2022-03-18 11:40:50.000000 celery-5.3.1/celery/app/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    23151 2023-02-02 09:58:18.000000 celery-5.3.1/celery/app/amqp.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1445 2021-10-12 14:26:47.000000 celery-5.3.1/celery/app/annotations.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2506 2023-06-18 13:06:44.000000 celery-5.3.1/celery/app/autoretry.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2702 2023-02-02 09:58:18.000000 celery-5.3.1/celery/app/backends.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    50088 2023-05-31 06:35:53.000000 celery-5.3.1/celery/app/base.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6673 2021-10-12 14:26:47.000000 celery-5.3.1/celery/app/builtins.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    29170 2023-02-02 09:58:18.000000 celery-5.3.1/celery/app/control.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    15014 2023-02-02 09:58:18.000000 celery-5.3.1/celery/app/defaults.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1326 2021-10-12 14:26:47.000000 celery-5.3.1/celery/app/events.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9067 2023-02-02 09:58:18.000000 celery-5.3.1/celery/app/log.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2001 2021-10-12 14:26:47.000000 celery-5.3.1/celery/app/registry.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4527 2021-10-12 14:26:47.000000 celery-5.3.1/celery/app/routes.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    43264 2023-05-31 06:35:53.000000 celery-5.3.1/celery/app/task.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    28320 2023-05-31 06:35:53.000000 celery-5.3.1/celery/app/trace.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    13160 2022-07-28 12:22:51.000000 celery-5.3.1/celery/app/utils.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.670497 celery-5.3.1/celery/apps/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/celery/apps/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5724 2023-05-31 06:35:53.000000 celery-5.3.1/celery/apps/beat.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    16360 2022-03-18 11:40:50.000000 celery-5.3.1/celery/apps/multi.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    13208 2023-02-02 09:58:18.000000 celery-5.3.1/celery/apps/worker.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.674497 celery-5.3.1/celery/backends/
+-rw-rw-r--   0 asif      (1000) asif      (1000)       23 2021-10-12 14:26:47.000000 celery-5.3.1/celery/backends/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7739 2022-06-29 10:52:39.000000 celery-5.3.1/celery/backends/arangodb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10309 2021-11-21 13:37:38.000000 celery-5.3.1/celery/backends/asynchronous.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5127 2022-03-18 11:40:50.000000 celery-5.3.1/celery/backends/azureblockblob.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    43970 2023-05-31 06:35:53.000000 celery-5.3.1/celery/backends/base.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4817 2021-10-12 14:26:47.000000 celery-5.3.1/celery/backends/cache.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9006 2023-02-02 09:58:18.000000 celery-5.3.1/celery/backends/cassandra.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3816 2021-10-12 14:26:47.000000 celery-5.3.1/celery/backends/consul.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6777 2023-02-02 09:58:18.000000 celery-5.3.1/celery/backends/cosmosdbsql.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3393 2022-06-29 10:52:39.000000 celery-5.3.1/celery/backends/couchbase.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2935 2021-10-12 14:26:47.000000 celery-5.3.1/celery/backends/couchdb.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.674497 celery-5.3.1/celery/backends/database/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7751 2023-02-02 09:58:18.000000 celery-5.3.1/celery/backends/database/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3351 2021-10-12 14:26:47.000000 celery-5.3.1/celery/backends/database/models.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3011 2021-10-12 14:26:47.000000 celery-5.3.1/celery/backends/database/session.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    17179 2023-02-02 09:58:18.000000 celery-5.3.1/celery/backends/dynamodb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8319 2023-02-02 09:58:18.000000 celery-5.3.1/celery/backends/elasticsearch.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3776 2022-06-29 10:52:39.000000 celery-5.3.1/celery/backends/filesystem.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10666 2023-02-02 09:58:18.000000 celery-5.3.1/celery/backends/mongodb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    26389 2023-02-02 09:58:18.000000 celery-5.3.1/celery/backends/redis.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    12077 2021-10-12 14:26:47.000000 celery-5.3.1/celery/backends/rpc.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2752 2021-10-12 14:26:47.000000 celery-5.3.1/celery/backends/s3.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    24338 2023-02-02 09:58:18.000000 celery-5.3.1/celery/beat.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.674497 celery-5.3.1/celery/bin/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/celery/bin/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10023 2022-06-29 10:52:39.000000 celery-5.3.1/celery/bin/amqp.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8525 2023-05-31 06:35:53.000000 celery-5.3.1/celery/bin/base.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2592 2022-07-28 12:22:51.000000 celery-5.3.1/celery/bin/beat.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2370 2022-03-18 11:40:50.000000 celery-5.3.1/celery/bin/call.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7317 2023-05-31 06:35:39.000000 celery-5.3.1/celery/bin/celery.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7058 2022-03-18 11:40:50.000000 celery-5.3.1/celery/bin/control.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2794 2022-03-18 11:40:50.000000 celery-5.3.1/celery/bin/events.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5796 2021-10-12 14:26:47.000000 celery-5.3.1/celery/bin/graph.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1058 2021-10-12 14:26:47.000000 celery-5.3.1/celery/bin/list.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4267 2021-10-12 14:26:47.000000 celery-5.3.1/celery/bin/logtool.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2108 2022-03-18 11:40:50.000000 celery-5.3.1/celery/bin/migrate.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    15364 2023-05-31 06:35:39.000000 celery-5.3.1/celery/bin/multi.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2547 2022-03-18 11:40:50.000000 celery-5.3.1/celery/bin/purge.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      976 2022-03-18 11:40:50.000000 celery-5.3.1/celery/bin/result.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4778 2023-05-31 06:35:39.000000 celery-5.3.1/celery/bin/shell.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3064 2022-03-18 11:40:50.000000 celery-5.3.1/celery/bin/upgrade.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    12886 2023-06-18 13:06:44.000000 celery-5.3.1/celery/bin/worker.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    12277 2023-02-02 09:58:18.000000 celery-5.3.1/celery/bootsteps.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    95874 2023-05-31 06:35:53.000000 celery-5.3.1/celery/canvas.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.678497 celery-5.3.1/celery/concurrency/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1457 2023-02-02 09:58:18.000000 celery-5.3.1/celery/concurrency/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    51471 2023-05-31 06:35:53.000000 celery-5.3.1/celery/concurrency/asynpool.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4706 2023-02-02 09:58:18.000000 celery-5.3.1/celery/concurrency/base.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5126 2021-10-12 14:26:47.000000 celery-5.3.1/celery/concurrency/eventlet.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3387 2023-02-02 09:58:18.000000 celery-5.3.1/celery/concurrency/gevent.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5850 2023-02-02 09:58:18.000000 celery-5.3.1/celery/concurrency/prefork.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      754 2023-02-02 09:58:18.000000 celery-5.3.1/celery/concurrency/solo.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1807 2023-06-03 16:07:04.000000 celery-5.3.1/celery/concurrency/thread.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.678497 celery-5.3.1/celery/contrib/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/celery/contrib/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5003 2022-03-18 11:40:50.000000 celery-5.3.1/celery/contrib/abortable.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    14361 2022-04-28 06:12:03.000000 celery-5.3.1/celery/contrib/migrate.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6754 2023-02-02 09:58:18.000000 celery-5.3.1/celery/contrib/pytest.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5005 2022-06-29 10:52:39.000000 celery-5.3.1/celery/contrib/rdb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3391 2023-02-02 09:58:18.000000 celery-5.3.1/celery/contrib/sphinx.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.678497 celery-5.3.1/celery/contrib/testing/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/celery/contrib/testing/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3112 2022-06-29 10:52:39.000000 celery-5.3.1/celery/contrib/testing/app.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7739 2023-02-02 09:58:18.000000 celery-5.3.1/celery/contrib/testing/manager.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4182 2023-02-02 09:58:18.000000 celery-5.3.1/celery/contrib/testing/mocks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      208 2021-10-12 14:26:47.000000 celery-5.3.1/celery/contrib/testing/tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5792 2023-02-02 09:58:18.000000 celery-5.3.1/celery/contrib/testing/worker.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.678497 celery-5.3.1/celery/events/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      477 2021-10-12 14:26:47.000000 celery-5.3.1/celery/events/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    17961 2022-06-29 10:52:39.000000 celery-5.3.1/celery/events/cursesmon.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8987 2021-10-12 14:26:47.000000 celery-5.3.1/celery/events/dispatcher.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3116 2021-10-12 14:26:47.000000 celery-5.3.1/celery/events/dumper.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1736 2021-10-12 14:26:47.000000 celery-5.3.1/celery/events/event.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4998 2021-10-12 14:26:47.000000 celery-5.3.1/celery/events/receiver.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3294 2021-10-12 14:26:47.000000 celery-5.3.1/celery/events/snapshot.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    25648 2023-02-02 09:58:18.000000 celery-5.3.1/celery/events/state.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9086 2023-05-31 06:35:53.000000 celery-5.3.1/celery/exceptions.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.682497 celery-5.3.1/celery/fixups/
+-rw-rw-r--   0 asif      (1000) asif      (1000)       14 2021-10-12 14:26:47.000000 celery-5.3.1/celery/fixups/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7161 2023-02-02 09:58:18.000000 celery-5.3.1/celery/fixups/django.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.682497 celery-5.3.1/celery/loaders/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      490 2021-10-12 14:26:47.000000 celery-5.3.1/celery/loaders/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      199 2021-10-12 14:26:47.000000 celery-5.3.1/celery/loaders/app.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8825 2022-03-18 11:40:50.000000 celery-5.3.1/celery/loaders/base.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1520 2021-10-12 14:26:47.000000 celery-5.3.1/celery/loaders/default.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    16087 2023-02-02 09:58:18.000000 celery-5.3.1/celery/local.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    25290 2023-02-02 09:58:18.000000 celery-5.3.1/celery/platforms.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    35282 2023-05-31 06:35:53.000000 celery-5.3.1/celery/result.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    32003 2023-05-31 06:35:53.000000 celery-5.3.1/celery/schedules.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.682497 celery-5.3.1/celery/security/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2363 2022-03-18 11:40:50.000000 celery-5.3.1/celery/security/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4008 2023-05-31 06:35:53.000000 celery-5.3.1/celery/security/certificate.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1189 2023-02-02 09:58:18.000000 celery-5.3.1/celery/security/key.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4248 2022-03-18 11:40:50.000000 celery-5.3.1/celery/security/serialization.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      845 2021-10-12 14:26:47.000000 celery-5.3.1/celery/security/utils.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4384 2023-05-31 06:35:53.000000 celery-5.3.1/celery/signals.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3324 2022-04-28 06:12:03.000000 celery-5.3.1/celery/states.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.686497 celery-5.3.1/celery/utils/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      935 2021-10-12 14:26:47.000000 celery-5.3.1/celery/utils/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2874 2021-10-12 14:26:47.000000 celery-5.3.1/celery/utils/abstract.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    25454 2023-06-18 13:06:44.000000 celery-5.3.1/celery/utils/collections.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4709 2021-10-12 14:26:47.000000 celery-5.3.1/celery/utils/debug.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3620 2021-10-12 14:26:47.000000 celery-5.3.1/celery/utils/deprecated.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.686497 celery-5.3.1/celery/utils/dispatch/
+-rw-rw-r--   0 asif      (1000) asif      (1000)       74 2021-10-12 14:26:47.000000 celery-5.3.1/celery/utils/dispatch/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    13603 2021-10-12 14:26:47.000000 celery-5.3.1/celery/utils/dispatch/signal.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    12017 2023-02-02 09:58:18.000000 celery-5.3.1/celery/utils/functional.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9041 2021-10-12 14:26:47.000000 celery-5.3.1/celery/utils/graph.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5032 2023-02-02 09:58:18.000000 celery-5.3.1/celery/utils/imports.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2871 2023-05-31 06:35:53.000000 celery-5.3.1/celery/utils/iso8601.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8757 2023-02-02 09:58:18.000000 celery-5.3.1/celery/utils/log.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2858 2021-10-12 14:26:47.000000 celery-5.3.1/celery/utils/nodenames.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4215 2021-10-12 14:26:47.000000 celery-5.3.1/celery/utils/objects.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8945 2023-02-02 09:58:18.000000 celery-5.3.1/celery/utils/saferepr.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8209 2023-05-31 06:35:53.000000 celery-5.3.1/celery/utils/serialization.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.686497 celery-5.3.1/celery/utils/static/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      299 2021-10-12 14:26:47.000000 celery-5.3.1/celery/utils/static/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2556 2021-10-12 14:26:47.000000 celery-5.3.1/celery/utils/static/celery_128.png
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1085 2021-10-12 14:26:47.000000 celery-5.3.1/celery/utils/sysinfo.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4532 2023-02-02 09:58:18.000000 celery-5.3.1/celery/utils/term.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5844 2023-05-31 06:35:53.000000 celery-5.3.1/celery/utils/text.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9552 2023-02-02 09:58:18.000000 celery-5.3.1/celery/utils/threads.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    14987 2023-05-31 06:35:53.000000 celery-5.3.1/celery/utils/time.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4813 2021-10-12 14:26:47.000000 celery-5.3.1/celery/utils/timer2.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.686497 celery-5.3.1/celery/worker/
+-rw-rw-r--   0 asif      (1000) asif      (1000)       95 2021-10-12 14:26:47.000000 celery-5.3.1/celery/worker/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4593 2021-10-12 14:26:47.000000 celery-5.3.1/celery/worker/autoscale.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7497 2023-02-02 09:58:18.000000 celery-5.3.1/celery/worker/components.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.690497 celery-5.3.1/celery/worker/consumer/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      391 2021-10-12 14:26:47.000000 celery-5.3.1/celery/worker/consumer/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      525 2021-10-12 14:26:47.000000 celery-5.3.1/celery/worker/consumer/agent.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1026 2021-10-12 14:26:47.000000 celery-5.3.1/celery/worker/consumer/connection.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    28320 2023-02-02 09:58:18.000000 celery-5.3.1/celery/worker/consumer/consumer.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      946 2021-10-12 14:26:47.000000 celery-5.3.1/celery/worker/consumer/control.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2054 2021-10-12 14:26:47.000000 celery-5.3.1/celery/worker/consumer/events.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6833 2021-10-12 14:26:47.000000 celery-5.3.1/celery/worker/consumer/gossip.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      930 2021-10-12 14:26:47.000000 celery-5.3.1/celery/worker/consumer/heart.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2519 2021-10-12 14:26:47.000000 celery-5.3.1/celery/worker/consumer/mingle.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1960 2022-03-18 11:40:50.000000 celery-5.3.1/celery/worker/consumer/tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    19884 2023-05-31 06:35:53.000000 celery-5.3.1/celery/worker/control.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2107 2021-10-12 14:26:47.000000 celery-5.3.1/celery/worker/heartbeat.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4433 2021-10-12 14:26:47.000000 celery-5.3.1/celery/worker/loops.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3630 2021-10-12 14:26:47.000000 celery-5.3.1/celery/worker/pidbox.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    27229 2023-05-31 06:35:53.000000 celery-5.3.1/celery/worker/request.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8583 2023-05-31 06:35:53.000000 celery-5.3.1/celery/worker/state.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7349 2021-10-12 14:26:47.000000 celery-5.3.1/celery/worker/strategy.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    14460 2023-02-02 09:58:18.000000 celery-5.3.1/celery/worker/worker.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.666497 celery-5.3.1/celery.egg-info/
+-rw-rw-r--   0 asif      (1000) asif      (1000)    18020 2023-06-18 14:18:33.000000 celery-5.3.1/celery.egg-info/PKG-INFO
+-rw-rw-r--   0 asif      (1000) asif      (1000)    21130 2023-06-18 14:18:33.000000 celery-5.3.1/celery.egg-info/SOURCES.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)        1 2023-06-18 14:18:33.000000 celery-5.3.1/celery.egg-info/dependency_links.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       49 2023-06-18 14:18:33.000000 celery-5.3.1/celery.egg-info/entry_points.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1833 2023-06-18 14:18:33.000000 celery-5.3.1/celery.egg-info/requires.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)        7 2023-06-18 14:18:33.000000 celery-5.3.1/celery.egg-info/top_level.txt
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.690497 celery-5.3.1/docs/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5293 2021-10-12 14:26:47.000000 celery-5.3.1/docs/AUTHORS.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8111 2021-10-12 14:26:47.000000 celery-5.3.1/docs/Makefile
+-rw-rw-r--   0 asif      (1000) asif      (1000)      494 2021-10-12 14:26:47.000000 celery-5.3.1/docs/THANKS
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.690497 celery-5.3.1/docs/_ext/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5164 2021-10-12 14:26:47.000000 celery-5.3.1/docs/_ext/celerydocs.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.690497 celery-5.3.1/docs/_static/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/docs/_static/.keep
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.690497 celery-5.3.1/docs/_templates/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      486 2021-10-12 14:26:47.000000 celery-5.3.1/docs/_templates/sidebardonations.html
+-rw-rw-r--   0 asif      (1000) asif      (1000)       30 2021-10-12 14:26:47.000000 celery-5.3.1/docs/changelog.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      981 2021-10-12 14:26:47.000000 celery-5.3.1/docs/community.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2597 2022-08-01 10:53:57.000000 celery-5.3.1/docs/conf.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)       83 2021-10-12 14:26:47.000000 celery-5.3.1/docs/configuration.html
+-rw-rw-r--   0 asif      (1000) asif      (1000)       33 2021-10-12 14:26:47.000000 celery-5.3.1/docs/contributing.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      931 2021-10-12 14:26:47.000000 celery-5.3.1/docs/copyright.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.690497 celery-5.3.1/docs/django/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7942 2023-06-18 13:06:44.000000 celery-5.3.1/docs/django/first-steps-with-django.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      137 2021-10-12 14:26:47.000000 celery-5.3.1/docs/django/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    29852 2023-05-31 06:35:53.000000 celery-5.3.1/docs/faq.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.690497 celery-5.3.1/docs/getting-started/
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.694497 celery-5.3.1/docs/getting-started/backends-and-brokers/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3903 2023-05-31 06:35:53.000000 celery-5.3.1/docs/getting-started/backends-and-brokers/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5010 2023-02-02 09:58:18.000000 celery-5.3.1/docs/getting-started/backends-and-brokers/rabbitmq.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7239 2023-05-31 06:35:53.000000 celery-5.3.1/docs/getting-started/backends-and-brokers/redis.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10843 2022-03-18 11:40:50.000000 celery-5.3.1/docs/getting-started/backends-and-brokers/sqs.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    14995 2023-02-02 09:58:18.000000 celery-5.3.1/docs/getting-started/first-steps-with-celery.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      226 2021-10-12 14:26:47.000000 celery-5.3.1/docs/getting-started/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10903 2023-06-18 13:06:44.000000 celery-5.3.1/docs/getting-started/introduction.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    22787 2022-08-01 10:53:57.000000 celery-5.3.1/docs/getting-started/next-steps.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      132 2021-10-12 14:26:47.000000 celery-5.3.1/docs/getting-started/resources.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4448 2021-10-12 14:26:47.000000 celery-5.3.1/docs/glossary.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.698498 celery-5.3.1/docs/history/
+-rw-rw-r--   0 asif      (1000) asif      (1000)    58104 2023-02-02 09:58:18.000000 celery-5.3.1/docs/history/changelog-1.0.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    34009 2022-08-01 10:53:57.000000 celery-5.3.1/docs/history/changelog-2.0.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    23550 2021-10-12 14:26:47.000000 celery-5.3.1/docs/history/changelog-2.1.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    33558 2022-08-01 10:53:57.000000 celery-5.3.1/docs/history/changelog-2.2.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    11200 2022-08-01 10:53:57.000000 celery-5.3.1/docs/history/changelog-2.3.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    13012 2022-08-01 10:53:57.000000 celery-5.3.1/docs/history/changelog-2.4.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5414 2021-10-12 14:26:47.000000 celery-5.3.1/docs/history/changelog-2.5.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    49344 2022-08-01 10:53:57.000000 celery-5.3.1/docs/history/changelog-3.0.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    52336 2022-08-01 10:53:57.000000 celery-5.3.1/docs/history/changelog-3.1.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6432 2021-10-12 14:26:47.000000 celery-5.3.1/docs/history/changelog-4.0.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8950 2021-10-12 14:26:47.000000 celery-5.3.1/docs/history/changelog-4.1.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    13593 2021-10-12 14:26:47.000000 celery-5.3.1/docs/history/changelog-4.2.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    17251 2021-10-12 14:26:47.000000 celery-5.3.1/docs/history/changelog-4.3.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    24332 2021-11-21 13:37:38.000000 celery-5.3.1/docs/history/changelog-4.4.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5720 2022-08-01 10:53:57.000000 celery-5.3.1/docs/history/changelog-5.0.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5592 2022-08-01 10:53:57.000000 celery-5.3.1/docs/history/changelog-5.1.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      675 2021-11-21 13:37:38.000000 celery-5.3.1/docs/history/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    16026 2021-10-12 14:26:47.000000 celery-5.3.1/docs/history/whatsnew-2.5.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    30892 2021-11-21 13:37:38.000000 celery-5.3.1/docs/history/whatsnew-3.0.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    44129 2021-10-12 14:26:47.000000 celery-5.3.1/docs/history/whatsnew-3.1.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    76466 2023-02-02 09:58:18.000000 celery-5.3.1/docs/history/whatsnew-4.0.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8244 2021-10-12 14:26:47.000000 celery-5.3.1/docs/history/whatsnew-4.1.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    35711 2021-10-12 14:26:47.000000 celery-5.3.1/docs/history/whatsnew-4.2.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    16865 2021-10-12 14:26:47.000000 celery-5.3.1/docs/history/whatsnew-4.3.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6999 2021-11-21 13:37:38.000000 celery-5.3.1/docs/history/whatsnew-4.4.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10957 2021-10-12 14:26:47.000000 celery-5.3.1/docs/history/whatsnew-5.0.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    14128 2023-02-02 09:58:18.000000 celery-5.3.1/docs/history/whatsnew-5.1.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.698498 celery-5.3.1/docs/images/
+-rw-rw-r--   0 asif      (1000) asif      (1000)    14168 2021-10-12 14:26:47.000000 celery-5.3.1/docs/images/celery-banner-small.png
+-rw-rw-r--   0 asif      (1000) asif      (1000)    14038 2021-10-12 14:26:47.000000 celery-5.3.1/docs/images/celery-banner.png
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2556 2021-10-12 14:26:47.000000 celery-5.3.1/docs/images/celery_128.png
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8658 2021-10-12 14:26:47.000000 celery-5.3.1/docs/images/celery_512.png
+-rw-rw-r--   0 asif      (1000) asif      (1000)    77397 2021-10-12 14:26:47.000000 celery-5.3.1/docs/images/celeryevshotsm.jpg
+-rw-rw-r--   0 asif      (1000) asif      (1000)    88879 2021-10-12 14:26:47.000000 celery-5.3.1/docs/images/dashboard.png
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4286 2021-10-12 14:26:47.000000 celery-5.3.1/docs/images/favicon.ico
+-rw-rw-r--   0 asif      (1000) asif      (1000)   146412 2021-10-12 14:26:47.000000 celery-5.3.1/docs/images/monitor.png
+-rw-rw-r--   0 asif      (1000) asif      (1000)    35894 2021-10-12 14:26:47.000000 celery-5.3.1/docs/images/result_graph.png
+-rw-rw-r--   0 asif      (1000) asif      (1000)    99783 2021-10-12 14:26:47.000000 celery-5.3.1/docs/images/worker_graph_full.png
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.698498 celery-5.3.1/docs/includes/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4023 2023-02-02 09:58:18.000000 celery-5.3.1/docs/includes/installation.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6420 2023-06-18 14:12:46.000000 celery-5.3.1/docs/includes/introduction.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1375 2023-02-02 09:58:18.000000 celery-5.3.1/docs/includes/resources.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1613 2021-11-21 13:37:38.000000 celery-5.3.1/docs/index.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.698498 celery-5.3.1/docs/internals/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5985 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/app-overview.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5696 2022-04-28 06:12:03.000000 celery-5.3.1/docs/internals/deprecation.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8586 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/guide.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      206 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9898 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/protocol.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.710498 celery-5.3.1/docs/internals/reference/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      226 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery._state.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      257 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.app.annotations.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      224 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.app.routes.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      239 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.app.trace.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.backends.arangodb.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.backends.asynchronous.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      293 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.backends.azureblockblob.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      243 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.backends.base.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      256 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.backends.cache.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      278 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.backends.cassandra.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      253 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.backends.consul.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      284 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.backends.cosmosdbsql.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      270 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.backends.couchbase.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      262 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.backends.couchdb.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      276 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.backends.database.models.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      293 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.backends.database.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      283 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.backends.database.session.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      265 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.backends.dynamodb.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      280 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.backends.elasticsearch.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      269 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.backends.filesystem.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      264 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.backends.mongodb.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      254 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.backends.redis.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      242 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.backends.rpc.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      206 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.backends.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      245 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.backends.s3.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      270 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.concurrency.base.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      310 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.concurrency.eventlet.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      304 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.concurrency.gevent.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      307 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.concurrency.prefork.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      229 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.concurrency.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      310 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.concurrency.solo.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      304 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.concurrency.thread.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      260 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.events.cursesmon.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      251 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.events.dumper.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      257 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.events.snapshot.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      231 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.platforms.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      272 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.security.certificate.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      248 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.security.key.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      278 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.security.serialization.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      254 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.security.utils.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      256 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.utils.abstract.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      252 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.utils.collections.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      260 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.utils.deprecated.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      252 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.utils.dispatch.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      295 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.utils.dispatch.signal.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      282 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.utils.functional.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      245 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.utils.graph.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      273 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.utils.imports.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.utils.iso8601.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      261 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.utils.log.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      257 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.utils.nodenames.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.utils.objects.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      195 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.utils.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      256 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.utils.saferepr.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      273 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.utils.serialization.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.utils.sysinfo.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      264 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.utils.term.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      264 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.utils.text.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      251 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.utils.threads.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      258 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.utils.time.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      224 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.utils.timer2.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      256 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.worker.autoscale.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      259 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.worker.components.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      260 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.worker.control.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      266 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.worker.heartbeat.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      236 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.worker.loops.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      239 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/celery.worker.pidbox.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1960 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/reference/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1452 2021-10-12 14:26:47.000000 celery-5.3.1/docs/internals/worker.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7675 2021-10-12 14:26:47.000000 celery-5.3.1/docs/make.bat
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.718498 celery-5.3.1/docs/reference/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1379 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.app.amqp.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      237 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.app.autoretry.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      234 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.app.backends.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      268 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.app.builtins.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      265 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.app.control.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      290 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.app.defaults.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      222 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.app.events.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      213 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.app.log.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      228 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.app.registry.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      288 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.app.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      226 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.app.task.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      219 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.app.utils.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      253 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.apps.beat.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      236 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.apps.multi.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      239 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.apps.worker.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      220 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.beat.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      189 2022-08-01 10:53:57.000000 celery-5.3.1/docs/reference/celery.bin.amqp.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      216 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.bin.base.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      254 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.bin.beat.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      258 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.bin.call.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      242 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.bin.celery.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.bin.control.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      264 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.bin.events.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      261 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.bin.graph.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      258 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.bin.list.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.bin.logtool.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.bin.migrate.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      249 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.bin.multi.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      261 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.bin.purge.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      264 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.bin.result.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      261 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.bin.shell.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.bin.upgrade.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      242 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.bin.worker.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      239 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.bootsteps.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      290 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.contrib.abortable.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      230 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.contrib.migrate.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      273 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.contrib.pytest.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      256 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.contrib.rdb.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      184 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.contrib.sphinx.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      288 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.contrib.testing.app.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      300 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.contrib.testing.manager.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.contrib.testing.mocks.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      297 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.contrib.testing.worker.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      304 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.events.dispatcher.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.events.event.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      303 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.events.receiver.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      194 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.events.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.events.state.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      222 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.exceptions.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      227 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.loaders.app.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      250 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.loaders.base.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      255 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.loaders.default.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      237 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.loaders.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      204 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.result.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3497 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      261 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.schedules.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      200 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.security.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      257 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.signals.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      106 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.states.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      871 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.utils.debug.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      291 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.worker.consumer.agent.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      306 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.worker.consumer.connection.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      300 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.worker.consumer.consumer.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      297 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.worker.consumer.control.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.worker.consumer.events.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.worker.consumer.gossip.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      291 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.worker.consumer.heart.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.worker.consumer.mingle.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      273 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.worker.consumer.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      291 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.worker.consumer.tasks.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      244 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.worker.request.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      226 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.worker.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      236 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.worker.state.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      245 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.worker.strategy.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      239 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/celery.worker.worker.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      143 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/cli.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1952 2021-10-12 14:26:47.000000 celery-5.3.1/docs/reference/index.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.718498 celery-5.3.1/docs/sec/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2921 2021-10-12 14:26:47.000000 celery-5.3.1/docs/sec/CELERYSA-0001.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2656 2021-10-12 14:26:47.000000 celery-5.3.1/docs/sec/CELERYSA-0002.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1551 2021-10-12 14:26:47.000000 celery-5.3.1/docs/sec/CELERYSA-0003.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4879 2021-10-12 14:26:47.000000 celery-5.3.1/docs/spelling_wordlist.txt
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.718498 celery-5.3.1/docs/templates/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1186 2023-02-02 09:58:18.000000 celery-5.3.1/docs/templates/readme.txt
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.718498 celery-5.3.1/docs/tutorials/
+-rw-rw-r--   0 asif      (1000) asif      (1000)       86 2021-10-12 14:26:47.000000 celery-5.3.1/docs/tutorials/daemonizing.html
+-rw-rw-r--   0 asif      (1000) asif      (1000)       91 2021-10-12 14:26:47.000000 celery-5.3.1/docs/tutorials/debugging.html
+-rw-rw-r--   0 asif      (1000) asif      (1000)      121 2021-10-12 14:26:47.000000 celery-5.3.1/docs/tutorials/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2766 2021-10-12 14:26:47.000000 celery-5.3.1/docs/tutorials/task-cookbook.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.722498 celery-5.3.1/docs/userguide/
+-rw-rw-r--   0 asif      (1000) asif      (1000)    14779 2022-04-28 06:12:03.000000 celery-5.3.1/docs/userguide/application.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    25233 2023-05-31 06:35:53.000000 celery-5.3.1/docs/userguide/calling.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    38007 2023-05-31 06:35:53.000000 celery-5.3.1/docs/userguide/canvas.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.722498 celery-5.3.1/docs/userguide/concurrency/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2665 2023-02-02 09:58:18.000000 celery-5.3.1/docs/userguide/concurrency/eventlet.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      140 2021-10-12 14:26:47.000000 celery-5.3.1/docs/userguide/concurrency/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    98436 2023-05-31 06:35:53.000000 celery-5.3.1/docs/userguide/configuration.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    17699 2023-02-02 09:58:18.000000 celery-5.3.1/docs/userguide/daemonizing.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3131 2021-10-12 14:26:47.000000 celery-5.3.1/docs/userguide/debugging.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    30057 2022-03-18 11:40:50.000000 celery-5.3.1/docs/userguide/extending.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      372 2021-10-12 14:26:47.000000 celery-5.3.1/docs/userguide/index.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    21759 2023-05-31 06:35:53.000000 celery-5.3.1/docs/userguide/monitoring.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8437 2021-12-29 05:20:59.000000 celery-5.3.1/docs/userguide/optimizing.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    20950 2023-05-31 06:35:53.000000 celery-5.3.1/docs/userguide/periodic-tasks.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    24323 2023-02-02 09:58:18.000000 celery-5.3.1/docs/userguide/routing.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8693 2022-07-28 12:22:51.000000 celery-5.3.1/docs/userguide/security.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    18113 2023-05-31 06:35:53.000000 celery-5.3.1/docs/userguide/signals.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      345 2021-10-12 14:26:47.000000 celery-5.3.1/docs/userguide/sphinx.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    64543 2023-02-02 09:58:18.000000 celery-5.3.1/docs/userguide/tasks.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    11146 2023-02-02 09:58:18.000000 celery-5.3.1/docs/userguide/testing.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    34758 2023-02-02 09:58:18.000000 celery-5.3.1/docs/userguide/workers.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)    11263 2023-06-06 05:40:38.000000 celery-5.3.1/docs/whatsnew-5.3.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.722498 celery-5.3.1/examples/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      303 2021-10-12 14:26:47.000000 celery-5.3.1/examples/README.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.722498 celery-5.3.1/examples/app/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      822 2022-06-29 10:52:39.000000 celery-5.3.1/examples/app/myapp.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.722498 celery-5.3.1/examples/celery_http_gateway/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1382 2021-10-12 14:26:47.000000 celery-5.3.1/examples/celery_http_gateway/README.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/examples/celery_http_gateway/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      385 2021-10-12 14:26:47.000000 celery-5.3.1/examples/celery_http_gateway/manage.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3001 2021-11-21 13:37:38.000000 celery-5.3.1/examples/celery_http_gateway/settings.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)       88 2021-10-12 14:26:47.000000 celery-5.3.1/examples/celery_http_gateway/tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      678 2022-03-18 11:40:50.000000 celery-5.3.1/examples/celery_http_gateway/urls.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.722498 celery-5.3.1/examples/django/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1546 2022-08-01 10:53:57.000000 celery-5.3.1/examples/django/README.rst
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.722498 celery-5.3.1/examples/django/demoapp/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/examples/django/demoapp/__init__.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.722498 celery-5.3.1/examples/django/demoapp/migrations/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      486 2021-10-12 14:26:47.000000 celery-5.3.1/examples/django/demoapp/migrations/0001_initial.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/examples/django/demoapp/migrations/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      103 2021-10-12 14:26:47.000000 celery-5.3.1/examples/django/demoapp/models.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      437 2021-10-12 14:26:47.000000 celery-5.3.1/examples/django/demoapp/tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)       26 2021-10-12 14:26:47.000000 celery-5.3.1/examples/django/demoapp/views.py
+-rwxrwxr-x   0 asif      (1000) asif      (1000)      248 2021-10-12 14:26:47.000000 celery-5.3.1/examples/django/manage.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.726498 celery-5.3.1/examples/django/proj/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      174 2021-10-12 14:26:47.000000 celery-5.3.1/examples/django/proj/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      659 2022-06-29 10:52:39.000000 celery-5.3.1/examples/django/proj/celery.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3639 2021-10-12 14:26:47.000000 celery-5.3.1/examples/django/proj/settings.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      556 2021-10-12 14:26:47.000000 celery-5.3.1/examples/django/proj/urls.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1132 2021-10-12 14:26:47.000000 celery-5.3.1/examples/django/proj/wsgi.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)       47 2023-02-02 09:58:18.000000 celery-5.3.1/examples/django/requirements.txt
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.726498 celery-5.3.1/examples/eventlet/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1449 2022-04-28 06:12:03.000000 celery-5.3.1/examples/eventlet/README.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1673 2021-10-12 14:26:47.000000 celery-5.3.1/examples/eventlet/bulk_task_producer.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      312 2022-04-28 06:12:03.000000 celery-5.3.1/examples/eventlet/celeryconfig.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      306 2022-04-28 06:12:03.000000 celery-5.3.1/examples/eventlet/tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2009 2022-04-28 06:12:03.000000 celery-5.3.1/examples/eventlet/webcrawler.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.726498 celery-5.3.1/examples/gevent/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      255 2021-10-12 14:26:47.000000 celery-5.3.1/examples/gevent/celeryconfig.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      325 2021-10-12 14:26:47.000000 celery-5.3.1/examples/gevent/tasks.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.726498 celery-5.3.1/examples/next-steps/
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.726498 celery-5.3.1/examples/next-steps/proj/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/examples/next-steps/proj/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.1/examples/next-steps/proj/celery.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      167 2021-10-12 14:26:47.000000 celery-5.3.1/examples/next-steps/proj/tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1224 2021-10-12 14:26:47.000000 celery-5.3.1/examples/next-steps/setup.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.726498 celery-5.3.1/examples/periodic-tasks/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1518 2022-08-01 10:53:57.000000 celery-5.3.1/examples/periodic-tasks/myapp.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.726498 celery-5.3.1/examples/resultgraph/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2860 2021-10-12 14:26:47.000000 celery-5.3.1/examples/resultgraph/tasks.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.726498 celery-5.3.1/examples/security/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1058 2021-10-12 14:26:47.000000 celery-5.3.1/examples/security/mysecureapp.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.726498 celery-5.3.1/examples/security/ssl/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3243 2021-10-12 14:26:47.000000 celery-5.3.1/examples/security/ssl/worker.key
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1923 2021-10-12 14:26:47.000000 celery-5.3.1/examples/security/ssl/worker.pem
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.726498 celery-5.3.1/examples/stamping/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      103 2023-02-02 09:58:18.000000 celery-5.3.1/examples/stamping/config.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1358 2023-05-31 06:35:53.000000 celery-5.3.1/examples/stamping/examples.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1806 2023-05-31 06:35:53.000000 celery-5.3.1/examples/stamping/myapp.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2548 2023-05-31 06:35:53.000000 celery-5.3.1/examples/stamping/revoke_example.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3311 2023-05-31 06:35:53.000000 celery-5.3.1/examples/stamping/tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2410 2023-05-31 06:35:53.000000 celery-5.3.1/examples/stamping/visitors.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.726498 celery-5.3.1/examples/tutorial/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      158 2021-10-12 14:26:47.000000 celery-5.3.1/examples/tutorial/tasks.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.662497 celery-5.3.1/extra/
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.726498 celery-5.3.1/extra/bash-completion/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      636 2021-10-12 14:26:47.000000 celery-5.3.1/extra/bash-completion/celery.bash
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.730498 celery-5.3.1/extra/generic-init.d/
+-rwxrwxr-x   0 asif      (1000) asif      (1000)     9068 2022-08-01 10:53:57.000000 celery-5.3.1/extra/generic-init.d/celerybeat
+-rwxrwxr-x   0 asif      (1000) asif      (1000)    10813 2023-05-31 06:35:53.000000 celery-5.3.1/extra/generic-init.d/celeryd
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.730498 celery-5.3.1/extra/macOS/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      751 2021-10-12 14:26:47.000000 celery-5.3.1/extra/macOS/org.celeryq.beat.plist
+-rw-rw-r--   0 asif      (1000) asif      (1000)      757 2021-10-12 14:26:47.000000 celery-5.3.1/extra/macOS/org.celeryq.worker.plist
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.730498 celery-5.3.1/extra/supervisord/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      134 2021-10-12 14:26:47.000000 celery-5.3.1/extra/supervisord/celery.sh
+-rw-rw-r--   0 asif      (1000) asif      (1000)      699 2021-10-12 14:26:47.000000 celery-5.3.1/extra/supervisord/celerybeat.conf
+-rw-rw-r--   0 asif      (1000) asif      (1000)      949 2021-10-12 14:26:47.000000 celery-5.3.1/extra/supervisord/celeryd.conf
+-rw-rw-r--   0 asif      (1000) asif      (1000)      982 2023-02-02 09:58:18.000000 celery-5.3.1/extra/supervisord/supervisord.conf
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.730498 celery-5.3.1/extra/systemd/
+-rw-rw-r--   0 asif      (1000) asif      (1000)      506 2022-08-01 10:53:57.000000 celery-5.3.1/extra/systemd/celery.conf
+-rw-rw-r--   0 asif      (1000) asif      (1000)      740 2021-10-12 14:26:47.000000 celery-5.3.1/extra/systemd/celery.service
+-rw-rw-r--   0 asif      (1000) asif      (1000)       78 2021-10-12 14:26:47.000000 celery-5.3.1/extra/systemd/celery.tmpfiles
+-rw-rw-r--   0 asif      (1000) asif      (1000)      395 2021-10-12 14:26:47.000000 celery-5.3.1/extra/systemd/celerybeat.service
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.730498 celery-5.3.1/extra/zsh-completion/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6244 2021-10-12 14:26:47.000000 celery-5.3.1/extra/zsh-completion/celery.zsh
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1216 2023-05-31 06:35:53.000000 celery-5.3.1/pyproject.toml
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.730498 celery-5.3.1/requirements/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1368 2023-06-06 05:40:26.000000 celery-5.3.1/requirements/README.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      273 2023-06-18 13:06:44.000000 celery-5.3.1/requirements/default.txt
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.730498 celery-5.3.1/requirements/deps/
+-rw-rw-r--   0 asif      (1000) asif      (1000)       10 2021-10-12 14:26:47.000000 celery-5.3.1/requirements/deps/mock.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      151 2023-05-31 06:35:53.000000 celery-5.3.1/requirements/dev.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      180 2023-06-18 13:06:44.000000 celery-5.3.1/requirements/docs.txt
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.738499 celery-5.3.1/requirements/extras/
+-rw-rw-r--   0 asif      (1000) asif      (1000)       16 2022-06-29 10:52:39.000000 celery-5.3.1/requirements/extras/arangodb.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       21 2023-06-03 16:07:04.000000 celery-5.3.1/requirements/extras/auth.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       28 2023-05-31 06:35:53.000000 celery-5.3.1/requirements/extras/azureblockblob.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      111 2021-10-12 14:26:47.000000 celery-5.3.1/requirements/extras/brotli.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       28 2022-06-29 10:52:39.000000 celery-5.3.1/requirements/extras/cassandra.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       22 2022-06-29 10:52:39.000000 celery-5.3.1/requirements/extras/consul.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       20 2022-04-28 06:12:03.000000 celery-5.3.1/requirements/extras/cosmosdbsql.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      119 2021-12-29 05:20:59.000000 celery-5.3.1/requirements/extras/couchbase.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       18 2022-06-29 10:52:39.000000 celery-5.3.1/requirements/extras/couchdb.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       15 2023-05-31 06:35:53.000000 celery-5.3.1/requirements/extras/django.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       16 2023-06-03 16:07:04.000000 celery-5.3.1/requirements/extras/dynamodb.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       18 2022-03-18 11:40:50.000000 celery-5.3.1/requirements/extras/elasticsearch.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       40 2021-11-21 13:37:38.000000 celery-5.3.1/requirements/extras/eventlet.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       14 2021-11-21 13:37:38.000000 celery-5.3.1/requirements/extras/gevent.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       44 2023-06-07 14:38:26.000000 celery-5.3.1/requirements/extras/librabbitmq.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       45 2023-02-02 09:58:18.000000 celery-5.3.1/requirements/extras/memcache.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       20 2022-04-28 06:12:03.000000 celery-5.3.1/requirements/extras/mongodb.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       15 2023-05-31 06:35:53.000000 celery-5.3.1/requirements/extras/msgpack.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       23 2022-04-28 06:12:03.000000 celery-5.3.1/requirements/extras/pymemcache.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       37 2023-06-18 13:49:41.000000 celery-5.3.1/requirements/extras/pyro.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       21 2022-06-29 10:52:39.000000 celery-5.3.1/requirements/extras/pytest.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       21 2023-06-18 13:06:44.000000 celery-5.3.1/requirements/extras/redis.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       16 2023-06-03 16:07:04.000000 celery-5.3.1/requirements/extras/s3.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       27 2021-10-12 14:26:47.000000 celery-5.3.1/requirements/extras/slmq.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       53 2023-05-31 06:35:53.000000 celery-5.3.1/requirements/extras/solar.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       27 2021-10-12 14:26:47.000000 celery-5.3.1/requirements/extras/sphinxautobuild.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       24 2023-05-31 06:35:53.000000 celery-5.3.1/requirements/extras/sqlalchemy.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      139 2023-06-07 14:38:26.000000 celery-5.3.1/requirements/extras/sqs.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       73 2021-10-12 14:26:47.000000 celery-5.3.1/requirements/extras/tblib.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       39 2021-10-12 14:26:47.000000 celery-5.3.1/requirements/extras/thread.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       13 2021-10-12 14:26:47.000000 celery-5.3.1/requirements/extras/yaml.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       14 2023-02-02 09:58:18.000000 celery-5.3.1/requirements/extras/zeromq.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       13 2021-10-12 14:26:47.000000 celery-5.3.1/requirements/extras/zookeeper.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       18 2023-05-31 06:35:53.000000 celery-5.3.1/requirements/extras/zstd.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      212 2023-05-31 06:35:53.000000 celery-5.3.1/requirements/pkgutils.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       19 2021-10-12 14:26:47.000000 celery-5.3.1/requirements/security.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      175 2023-05-31 06:35:53.000000 celery-5.3.1/requirements/test-ci-base.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      611 2023-06-07 14:38:26.000000 celery-5.3.1/requirements/test-ci-default.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      160 2023-05-31 06:35:53.000000 celery-5.3.1/requirements/test-integration.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)       17 2021-10-12 14:26:47.000000 celery-5.3.1/requirements/test-pypy3.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      306 2023-06-18 13:06:44.000000 celery-5.3.1/requirements/test.txt
+-rw-rw-r--   0 asif      (1000) asif      (1000)      486 2023-06-18 14:18:33.758499 celery-5.3.1/setup.cfg
+-rwxrwxr-x   0 asif      (1000) asif      (1000)     4559 2023-06-18 13:06:44.000000 celery-5.3.1/setup.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.738499 celery-5.3.1/t/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/t/__init__.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.738499 celery-5.3.1/t/benchmarks/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2816 2022-06-29 10:52:39.000000 celery-5.3.1/t/benchmarks/bench_worker.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.738499 celery-5.3.1/t/integration/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/t/integration/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2350 2023-02-02 09:58:18.000000 celery-5.3.1/t/integration/conftest.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    12427 2023-05-31 06:35:53.000000 celery-5.3.1/t/integration/tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1120 2021-10-12 14:26:47.000000 celery-5.3.1/t/integration/test_backend.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)   132248 2023-05-31 06:35:53.000000 celery-5.3.1/t/integration/test_canvas.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7796 2023-02-02 09:58:18.000000 celery-5.3.1/t/integration/test_inspect.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3459 2021-10-12 14:26:47.000000 celery-5.3.1/t/integration/test_security.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    18656 2023-05-31 06:35:53.000000 celery-5.3.1/t/integration/test_tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      688 2022-06-29 10:52:39.000000 celery-5.3.1/t/integration/test_worker.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      293 2022-06-29 10:52:39.000000 celery-5.3.1/t/integration/test_worker_config.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      226 2021-10-12 14:26:47.000000 celery-5.3.1/t/skip.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.738499 celery-5.3.1/t/unit/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/__init__.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.742499 celery-5.3.1/t/unit/app/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/app/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    13768 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/app/test_amqp.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1338 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/app/test_annotations.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    41390 2023-05-31 06:35:53.000000 celery-5.3.1/t/unit/app/test_app.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4542 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/app/test_backends.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    29065 2023-05-31 06:35:53.000000 celery-5.3.1/t/unit/app/test_beat.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5528 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/app/test_builtins.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      356 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/app/test_celery.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    19105 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/app/test_control.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1608 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/app/test_defaults.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      801 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/app/test_exceptions.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8823 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/app/test_loaders.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    11820 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/app/test_log.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2349 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/app/test_registry.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8026 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/app/test_routes.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    37835 2023-05-31 06:35:53.000000 celery-5.3.1/t/unit/app/test_schedules.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1790 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/app/test_utils.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.742499 celery-5.3.1/t/unit/apps/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/apps/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    16234 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/apps/test_multi.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.746499 celery-5.3.1/t/unit/backends/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/backends/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4362 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/backends/test_arangodb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6874 2021-11-21 13:37:38.000000 celery-5.3.1/t/unit/backends/test_asynchronous.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6794 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/backends/test_azureblockblob.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    45945 2023-05-31 06:35:53.000000 celery-5.3.1/t/unit/backends/test_base.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10318 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/backends/test_cache.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8669 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/backends/test_cassandra.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1448 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/backends/test_consul.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4994 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/backends/test_cosmosdbsql.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4846 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/backends/test_couchbase.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3971 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/backends/test_couchdb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    15087 2023-05-31 06:35:53.000000 celery-5.3.1/t/unit/backends/test_database.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    19214 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/backends/test_dynamodb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    32601 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/backends/test_elasticsearch.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4435 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/backends/test_filesystem.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    28352 2023-05-31 06:35:53.000000 celery-5.3.1/t/unit/backends/test_mongodb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    50595 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/backends/test_redis.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3692 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/backends/test_rpc.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6654 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/backends/test_s3.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.746499 celery-5.3.1/t/unit/bin/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/bin/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)       18 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/bin/celery.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.746499 celery-5.3.1/t/unit/bin/proj/
+-rw-rw-r--   0 asif      (1000) asif      (1000)       64 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/bin/proj/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      121 2022-06-29 10:52:39.000000 celery-5.3.1/t/unit/bin/proj/app.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)       22 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/bin/proj/app2.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      109 2022-07-28 12:22:51.000000 celery-5.3.1/t/unit/bin/proj/scheduler.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1116 2022-07-28 12:22:51.000000 celery-5.3.1/t/unit/bin/test_beat.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/bin/test_multi.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      529 2022-06-29 10:52:39.000000 celery-5.3.1/t/unit/bin/test_worker.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.746499 celery-5.3.1/t/unit/concurrency/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/concurrency/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5687 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/concurrency/test_concurrency.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     4721 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/concurrency/test_eventlet.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3146 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/concurrency/test_gevent.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1837 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/concurrency/test_pool.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    16398 2023-05-31 06:35:53.000000 celery-5.3.1/t/unit/concurrency/test_prefork.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      848 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/concurrency/test_solo.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      728 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/concurrency/test_thread.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    23214 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/conftest.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.746499 celery-5.3.1/t/unit/contrib/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/contrib/__init__.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.750499 celery-5.3.1/t/unit/contrib/proj/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/contrib/proj/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      183 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/contrib/proj/conf.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)       93 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/contrib/proj/contents.rst
+-rw-rw-r--   0 asif      (1000) asif      (1000)      249 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/contrib/proj/foo.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      113 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/contrib/proj/xyzzy.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1394 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/contrib/test_abortable.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10615 2022-03-18 11:40:50.000000 celery-5.3.1/t/unit/contrib/test_migrate.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      785 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/contrib/test_pytest.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3146 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/contrib/test_rdb.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      731 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/contrib/test_sphinx.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1474 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/contrib/test_worker.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.750499 celery-5.3.1/t/unit/events/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/events/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2304 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/events/test_cursesmon.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    11372 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/events/test_events.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3359 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/events/test_snapshot.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    22261 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/events/test_state.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.750499 celery-5.3.1/t/unit/fixups/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/fixups/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    11013 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/fixups/test_django.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.750499 celery-5.3.1/t/unit/security/
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7344 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/security/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      109 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/security/case.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3333 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/security/test_certificate.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1570 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/security/test_key.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6219 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/security/test_security.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2224 2022-03-18 11:40:50.000000 celery-5.3.1/t/unit/security/test_serialization.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.750499 celery-5.3.1/t/unit/tasks/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/tasks/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    68472 2023-05-31 06:35:53.000000 celery-5.3.1/t/unit/tasks/test_canvas.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    12308 2023-05-31 06:35:53.000000 celery-5.3.1/t/unit/tasks/test_chord.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3134 2022-06-29 10:52:39.000000 celery-5.3.1/t/unit/tasks/test_context.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    34984 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/tasks/test_result.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    52722 2023-05-31 06:35:53.000000 celery-5.3.1/t/unit/tasks/test_stamping.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1085 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/tasks/test_states.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    58015 2023-06-18 13:06:44.000000 celery-5.3.1/t/unit/tasks/test_tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    21991 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/tasks/test_trace.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)       78 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/tasks/unit_tasks.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      989 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/test_canvas.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.754499 celery-5.3.1/t/unit/utils/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/utils/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    13188 2023-06-18 13:06:44.000000 celery-5.3.1/t/unit/utils/test_collections.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2357 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/utils/test_debug.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1739 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/utils/test_deprecated.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5233 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/utils/test_dispatcher.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    13576 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/utils/test_functional.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1935 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/utils/test_graph.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3272 2022-03-18 11:40:50.000000 celery-5.3.1/t/unit/utils/test_imports.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     8515 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/utils/test_local.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      202 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/utils/test_nodenames.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      172 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/utils/test_objects.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1386 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/utils/test_pickle.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    32949 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/utils/test_platforms.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     5555 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/utils/test_saferepr.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3219 2023-05-31 06:35:53.000000 celery-5.3.1/t/unit/utils/test_serialization.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      751 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/utils/test_sysinfo.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1734 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/utils/test_term.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     1935 2022-03-18 11:40:50.000000 celery-5.3.1/t/unit/utils/test_text.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2427 2022-03-18 11:40:50.000000 celery-5.3.1/t/unit/utils/test_threads.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    11465 2023-05-31 06:35:53.000000 celery-5.3.1/t/unit/utils/test_time.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     3215 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/utils/test_timer2.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      624 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/utils/test_utils.py
+drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2023-06-18 14:18:33.758499 celery-5.3.1/t/unit/worker/
+-rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/worker/__init__.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     7574 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/worker/test_autoscale.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     9415 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/worker/test_bootsteps.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2461 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/worker/test_components.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    30428 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/worker/test_consumer.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    28334 2023-05-31 06:35:53.000000 celery-5.3.1/t/unit/worker/test_control.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     2384 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/worker/test_heartbeat.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    18256 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/worker/test_loops.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    48131 2023-05-31 06:35:53.000000 celery-5.3.1/t/unit/worker/test_request.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)      238 2021-10-12 14:26:47.000000 celery-5.3.1/t/unit/worker/test_revoke.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)     6339 2023-05-31 06:35:53.000000 celery-5.3.1/t/unit/worker/test_state.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    10989 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/worker/test_strategy.py
+-rw-rw-r--   0 asif      (1000) asif      (1000)    39912 2023-02-02 09:58:18.000000 celery-5.3.1/t/unit/worker/test_worker.py
```

### Comparing `celery-5.3.0rc2/CONTRIBUTORS.txt` & `celery-5.3.1/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/Changelog.rst` & `celery-5.3.1/Changelog.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,50 @@
 .. _changelog:
 
 ================
  Change history
 ================
 
 This document contains change notes for bugfix & new features
-in the main branch & 5.2.x series, please see :ref:`whatsnew-5.2` for
-an overview of what's new in Celery 5.2.
+in the main branch & 5.3.x series, please see :ref:`whatsnew-5.3` for
+an overview of what's new in Celery 5.3.
+
+
+.. _version-5.3.1:
+
+5.3.1
+=====
+
+:release-date: 2023-06-18  8:15 P.M GMT+6
+:release-by: Asif Saif Uddin
+
+- Upgrade to latest pycurl release (#7069).
+- Limit librabbitmq>=2.0.0; python_version < '3.11' (#8302).
+- Added initial support for python 3.11 (#8304).
+- ChainMap observers fix (#8305).
+- Revert optimization CLI flag behaviour back to original.
+- Restrict redis 4.5.5 as it has severe bugs (#8317).
+- Tested pypy 3.10 version in CI (#8320).
+- Bump new version of kombu to 5.3.1 (#8323).
+- Fixed a small float value of retry_backoff (#8295).
+- Limit pyro4 up to python 3.10 only as it is (#8324).
+
+
+
+.. _version-5.3.0:
+
+5.3.0
+=====
+
+:release-date: 2023-06-06 12:00 P.M GMT+6
+:release-by: Asif Saif Uddin
+
+- Test kombu 5.3.0 & minor doc update (#8294).
+- Update librabbitmq.txt > 2.0.0 (#8292).
+- Upgrade syntax to py3.8 (#8281).
 
 
 .. _version-5.3.0rc2:
 
 5.3.0rc2
 ========
```

### Comparing `celery-5.3.0rc2/LICENSE` & `celery-5.3.1/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-Copyright (c) 2015-2016 Ask Solem & contributors.  All rights reserved.
+Copyright (c) 2017-2026 Asif Saif Uddin, core team & contributors. All rights reserved.
+Copyright (c) 2015-2016 Ask Solem & contributors. All rights reserved.
 Copyright (c) 2012-2014 GoPivotal, Inc.  All rights reserved.
-Copyright (c) 2009, 2010, 2011, 2012 Ask Solem, and individual contributors.  All rights reserved.
+Copyright (c) 2009, 2010, 2011, 2012 Ask Solem, and individual contributors. All rights reserved.
 
 Celery is licensed under The BSD License (3 Clause, also known as
 the new BSD license).  The license is an OSI approved Open Source
 license and is GPL-compatible(1).
 
 The license text can also be found here:
 http://www.opensource.org/licenses/BSD-3-Clause
```

### Comparing `celery-5.3.0rc2/MANIFEST.in` & `celery-5.3.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/PKG-INFO` & `celery-5.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celery
-Version: 5.3.0rc2
+Version: 5.3.1
 Summary: Distributed Task Queue.
 Home-page: https://docs.celeryq.dev/
 Author: Ask Solem
 Author-email: auvipy@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.celeryq.dev/en/stable/
 Project-URL: Changelog, https://docs.celeryq.dev/en/stable/changelog.html
@@ -19,18 +19,19 @@
 Classifier: Topic :: Software Development :: Object Brokering
 Classifier: Framework :: Celery
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: arangodb
 Provides-Extra: auth
 Provides-Extra: azureblockblob
 Provides-Extra: brotli
 Provides-Extra: cassandra
 Provides-Extra: consul
 Provides-Extra: cosmosdbsql
@@ -60,15 +61,15 @@
 Provides-Extra: zstd
 License-File: LICENSE
 
 .. image:: https://docs.celeryq.dev/en/latest/_images/celery-banner-small.png
 
 |build-status| |coverage| |license| |wheel| |semgrep| |pyversion| |pyimp| |ocbackerbadge| |ocsponsorbadge|
 
-:Version: 5.3.0rc2 (dawn-chorus)
+:Version: 5.3.1 (emerald-rush)
 :Web: https://docs.celeryq.dev/en/stable/index.html
 :Download: https://pypi.org/project/celery/
 :Source: https://github.com/celery/celery/
 :Keywords: task, queue, job, async, rabbitmq, amqp, redis,
   python, distributed, actors
 
 Donations
@@ -116,48 +117,49 @@
 .. _`gocelery`: https://github.com/gocelery/gocelery
 .. _gopher-celery: https://github.com/marselester/gopher-celery
 .. _rusty-celery: https://github.com/rusty-celery/rusty-celery
 
 What do I need?
 ===============
 
-Celery version 5.3.0a1 runs on,
+Celery version 5.3.1 runs on,
 
-- Python (3.8, 3.9, 3.10)
+- Python (3.8, 3.9, 3.10, 3.11)
 - PyPy3.8+ (v7.3.11+)
 
 
-This is the version of celery which will support Python 3.7 or newer.
+This is the version of celery which will support Python 3.8 or newer.
 
 If you're running an older version of Python, you need to be running
 an older version of Celery:
 
+- Python 3.7: Celery 5.2 or earlier.
 - Python 3.6: Celery 5.1 or earlier.
 - Python 2.7: Celery 4.x series.
 - Python 2.6: Celery series 3.1 or earlier.
 - Python 2.5: Celery series 3.0 or earlier.
 - Python 2.4: Celery series 2.2 or earlier.
 
 Celery is a project with minimal funding,
-so we don't support Microsoft Windows.
+so we don't support Microsoft Windows but it should be working.
 Please don't open any issues related to that platform.
 
 *Celery* is usually used with a message broker to send and receive messages.
 The RabbitMQ, Redis transports are feature complete,
 but there's also experimental support for a myriad of other solutions, including
 using SQLite for local development.
 
 *Celery* can run on a single machine, on multiple machines, or even
 across datacenters.
 
 Get Started
 ===========
 
 If this is the first time you're trying to use Celery, or you're
-new to Celery v5.3.0a1 coming from previous versions then you should read our
+new to Celery v5.3.1 coming from previous versions then you should read our
 getting started tutorials:
 
 - `First steps with Celery`_
 
     Tutorial teaching you the bare minimum needed to get started with Celery.
 
 - `Next steps`_
@@ -317,17 +319,17 @@
 You can specify these in your requirements or on the ``pip``
 command-line by using brackets. Multiple bundles can be specified by
 separating them by commas.
 
 ::
 
 
-    $ pip install "celery[amqp]"
+    $ pip install "celery[redis]"
 
-    $ pip install "celery[amqp,redis,auth,msgpack]"
+    $ pip install "celery[redis,auth,msgpack]"
 
 The following bundles are available:
 
 Serializers
 ~~~~~~~~~~~
 
 :``celery[auth]``:
```

### Comparing `celery-5.3.0rc2/README.rst` & `celery-5.3.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 .. image:: https://docs.celeryq.dev/en/latest/_images/celery-banner-small.png
 
 |build-status| |coverage| |license| |wheel| |semgrep| |pyversion| |pyimp| |ocbackerbadge| |ocsponsorbadge|
 
-:Version: 5.3.0rc2 (dawn-chorus)
+:Version: 5.3.1 (emerald-rush)
 :Web: https://docs.celeryq.dev/en/stable/index.html
 :Download: https://pypi.org/project/celery/
 :Source: https://github.com/celery/celery/
 :Keywords: task, queue, job, async, rabbitmq, amqp, redis,
   python, distributed, actors
 
 Donations
@@ -54,48 +54,49 @@
 .. _`gocelery`: https://github.com/gocelery/gocelery
 .. _gopher-celery: https://github.com/marselester/gopher-celery
 .. _rusty-celery: https://github.com/rusty-celery/rusty-celery
 
 What do I need?
 ===============
 
-Celery version 5.3.0a1 runs on,
+Celery version 5.3.1 runs on,
 
-- Python (3.8, 3.9, 3.10)
+- Python (3.8, 3.9, 3.10, 3.11)
 - PyPy3.8+ (v7.3.11+)
 
 
-This is the version of celery which will support Python 3.7 or newer.
+This is the version of celery which will support Python 3.8 or newer.
 
 If you're running an older version of Python, you need to be running
 an older version of Celery:
 
+- Python 3.7: Celery 5.2 or earlier.
 - Python 3.6: Celery 5.1 or earlier.
 - Python 2.7: Celery 4.x series.
 - Python 2.6: Celery series 3.1 or earlier.
 - Python 2.5: Celery series 3.0 or earlier.
 - Python 2.4: Celery series 2.2 or earlier.
 
 Celery is a project with minimal funding,
-so we don't support Microsoft Windows.
+so we don't support Microsoft Windows but it should be working.
 Please don't open any issues related to that platform.
 
 *Celery* is usually used with a message broker to send and receive messages.
 The RabbitMQ, Redis transports are feature complete,
 but there's also experimental support for a myriad of other solutions, including
 using SQLite for local development.
 
 *Celery* can run on a single machine, on multiple machines, or even
 across datacenters.
 
 Get Started
 ===========
 
 If this is the first time you're trying to use Celery, or you're
-new to Celery v5.3.0a1 coming from previous versions then you should read our
+new to Celery v5.3.1 coming from previous versions then you should read our
 getting started tutorials:
 
 - `First steps with Celery`_
 
     Tutorial teaching you the bare minimum needed to get started with Celery.
 
 - `Next steps`_
@@ -255,17 +256,17 @@
 You can specify these in your requirements or on the ``pip``
 command-line by using brackets. Multiple bundles can be specified by
 separating them by commas.
 
 ::
 
 
-    $ pip install "celery[amqp]"
+    $ pip install "celery[redis]"
 
-    $ pip install "celery[amqp,redis,auth,msgpack]"
+    $ pip install "celery[redis,auth,msgpack]"
 
 The following bundles are available:
 
 Serializers
 ~~~~~~~~~~~
 
 :``celery[auth]``:
```

### Comparing `celery-5.3.0rc2/celery/__init__.py` & `celery-5.3.1/celery/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Distributed Task Queue."""
-# :copyright: (c) 2016-2026 Asif Saif Uddin, celery core and individual
+# :copyright: (c) 2017-2026 Asif Saif Uddin, celery core and individual
 #                 contributors, All rights reserved.
 # :copyright: (c) 2015-2016 Ask Solem.  All rights reserved.
 # :copyright: (c) 2012-2014 GoPivotal, Inc., All rights reserved.
 # :copyright: (c) 2009 - 2012 Ask Solem and individual contributors,
 #                 All rights reserved.
 # :license:   BSD (3 Clause), see LICENSE for more details.
 
@@ -11,17 +11,17 @@
 import re
 import sys
 from collections import namedtuple
 
 # Lazy loading
 from . import local
 
-SERIES = 'dawn-chorus'
+SERIES = 'emerald-rush'
 
-__version__ = '5.3.0rc2'
+__version__ = '5.3.1'
 __author__ = 'Ask Solem'
 __contact__ = 'auvipy@gmail.com'
 __homepage__ = 'https://docs.celeryq.dev/'
 __docformat__ = 'restructuredtext'
 __keywords__ = 'task job queue distributed messaging actor'
 
 # -eof meta-
```

### Comparing `celery-5.3.0rc2/celery/_state.py` & `celery-5.3.1/celery/_state.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/app/__init__.py` & `celery-5.3.1/celery/app/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/app/amqp.py` & `celery-5.3.1/celery/app/amqp.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/app/annotations.py` & `celery-5.3.1/celery/app/annotations.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/app/autoretry.py` & `celery-5.3.1/celery/app/autoretry.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     dont_autoretry_for = tuple(
         options.get('dont_autoretry_for',
                     getattr(task, 'dont_autoretry_for', ()))
     )
     retry_kwargs = options.get(
         'retry_kwargs', getattr(task, 'retry_kwargs', {})
     )
-    retry_backoff = int(
+    retry_backoff = float(
         options.get('retry_backoff',
                     getattr(task, 'retry_backoff', False))
     )
     retry_backoff_max = int(
         options.get('retry_backoff_max',
                     getattr(task, 'retry_backoff_max', 600))
     )
@@ -44,15 +44,15 @@
                 raise
             except dont_autoretry_for:
                 raise
             except autoretry_for as exc:
                 if retry_backoff:
                     retry_kwargs['countdown'] = \
                         get_exponential_backoff_interval(
-                            factor=retry_backoff,
+                            factor=int(max(1.0, retry_backoff)),
                             retries=task.request.retries,
                             maximum=retry_backoff_max,
                             full_jitter=retry_jitter)
                 # Override max_retries
                 if hasattr(task, 'override_max_retries'):
                     retry_kwargs['max_retries'] = getattr(task,
                                                           'override_max_retries',
```

### Comparing `celery-5.3.0rc2/celery/app/backends.py` & `celery-5.3.1/celery/app/backends.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/app/base.py` & `celery-5.3.1/celery/app/base.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/app/builtins.py` & `celery-5.3.1/celery/app/builtins.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/app/control.py` & `celery-5.3.1/celery/app/control.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/app/defaults.py` & `celery-5.3.1/celery/app/defaults.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/app/events.py` & `celery-5.3.1/celery/app/events.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/app/log.py` & `celery-5.3.1/celery/app/log.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/app/registry.py` & `celery-5.3.1/celery/app/registry.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/app/routes.py` & `celery-5.3.1/celery/app/routes.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/app/task.py` & `celery-5.3.1/celery/app/task.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/app/trace.py` & `celery-5.3.1/celery/app/trace.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/app/utils.py` & `celery-5.3.1/celery/app/utils.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/apps/beat.py` & `celery-5.3.1/celery/apps/beat.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/apps/multi.py` & `celery-5.3.1/celery/apps/multi.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/apps/worker.py` & `celery-5.3.1/celery/apps/worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/backends/arangodb.py` & `celery-5.3.1/celery/backends/arangodb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/backends/asynchronous.py` & `celery-5.3.1/celery/backends/asynchronous.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/backends/azureblockblob.py` & `celery-5.3.1/celery/backends/azureblockblob.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/backends/base.py` & `celery-5.3.1/celery/backends/base.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/backends/cache.py` & `celery-5.3.1/celery/backends/cache.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/backends/cassandra.py` & `celery-5.3.1/celery/backends/cassandra.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/backends/consul.py` & `celery-5.3.1/celery/backends/consul.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/backends/cosmosdbsql.py` & `celery-5.3.1/celery/backends/cosmosdbsql.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/backends/couchbase.py` & `celery-5.3.1/celery/backends/couchbase.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/backends/couchdb.py` & `celery-5.3.1/celery/backends/couchdb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/backends/database/__init__.py` & `celery-5.3.1/celery/backends/database/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/backends/database/models.py` & `celery-5.3.1/celery/backends/database/models.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/backends/database/session.py` & `celery-5.3.1/celery/backends/database/session.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/backends/dynamodb.py` & `celery-5.3.1/celery/backends/dynamodb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/backends/elasticsearch.py` & `celery-5.3.1/celery/backends/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/backends/filesystem.py` & `celery-5.3.1/celery/backends/filesystem.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/backends/mongodb.py` & `celery-5.3.1/celery/backends/mongodb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/backends/redis.py` & `celery-5.3.1/celery/backends/redis.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/backends/rpc.py` & `celery-5.3.1/celery/backends/rpc.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/backends/s3.py` & `celery-5.3.1/celery/backends/s3.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/beat.py` & `celery-5.3.1/celery/beat.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/bin/amqp.py` & `celery-5.3.1/celery/bin/amqp.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/bin/base.py` & `celery-5.3.1/celery/bin/base.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/bin/beat.py` & `celery-5.3.1/celery/bin/beat.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/bin/call.py` & `celery-5.3.1/celery/bin/call.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/bin/celery.py` & `celery-5.3.1/celery/bin/celery.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/bin/control.py` & `celery-5.3.1/celery/bin/control.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/bin/events.py` & `celery-5.3.1/celery/bin/events.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/bin/graph.py` & `celery-5.3.1/celery/bin/graph.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/bin/list.py` & `celery-5.3.1/celery/bin/list.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/bin/logtool.py` & `celery-5.3.1/celery/bin/logtool.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/bin/migrate.py` & `celery-5.3.1/celery/bin/migrate.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/bin/multi.py` & `celery-5.3.1/celery/bin/multi.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/bin/purge.py` & `celery-5.3.1/celery/bin/purge.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/bin/result.py` & `celery-5.3.1/celery/bin/result.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/bin/shell.py` & `celery-5.3.1/celery/bin/shell.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/bin/upgrade.py` & `celery-5.3.1/celery/bin/upgrade.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/bin/worker.py` & `celery-5.3.1/celery/bin/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,16 +162,16 @@
 @click.option('-l',
               '--loglevel',
               default='WARNING',
               cls=CeleryOption,
               type=LOG_LEVEL,
               help_group="Worker Options",
               help="Logging level.")
-@click.option('optimization',
-              '-O',
+@click.option('-O',
+              '--optimization',
               default='default',
               cls=CeleryOption,
               type=click.Choice(('default', 'fair')),
               help_group="Worker Options",
               help="Apply optimization profile.")
 @click.option('--prefetch-multiplier',
               type=int,
```

### Comparing `celery-5.3.0rc2/celery/bootsteps.py` & `celery-5.3.1/celery/bootsteps.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/canvas.py` & `celery-5.3.1/celery/canvas.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/concurrency/__init__.py` & `celery-5.3.1/celery/concurrency/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/concurrency/asynpool.py` & `celery-5.3.1/celery/concurrency/asynpool.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/concurrency/base.py` & `celery-5.3.1/celery/concurrency/base.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/concurrency/eventlet.py` & `celery-5.3.1/celery/concurrency/eventlet.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/concurrency/gevent.py` & `celery-5.3.1/celery/concurrency/gevent.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/concurrency/prefork.py` & `celery-5.3.1/celery/concurrency/prefork.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/concurrency/solo.py` & `celery-5.3.1/celery/concurrency/solo.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/concurrency/thread.py` & `celery-5.3.1/celery/concurrency/thread.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,15 @@
 from typing import TYPE_CHECKING, Any, Callable
 
 from .base import BasePool, apply_target
 
 __all__ = ('TaskPool',)
 
 if TYPE_CHECKING:
-    import sys
-
-    if sys.version_info >= (3, 8):
-        from typing import TypedDict
-    else:
-        from typing_extensions import TypedDict
+    from typing import TypedDict
 
     PoolInfo = TypedDict('PoolInfo', {'max-concurrency': int, 'threads': int})
 
     # `TargetFunction` should be a Protocol that represents fast_trace_task and
     # trace_task_ret.
     TargetFunction = Callable[..., Any]
```

### Comparing `celery-5.3.0rc2/celery/contrib/abortable.py` & `celery-5.3.1/celery/contrib/abortable.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/contrib/migrate.py` & `celery-5.3.1/celery/contrib/migrate.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/contrib/pytest.py` & `celery-5.3.1/celery/contrib/pytest.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/contrib/rdb.py` & `celery-5.3.1/celery/contrib/rdb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/contrib/sphinx.py` & `celery-5.3.1/celery/contrib/sphinx.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/contrib/testing/app.py` & `celery-5.3.1/celery/contrib/testing/app.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/contrib/testing/manager.py` & `celery-5.3.1/celery/contrib/testing/manager.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/contrib/testing/mocks.py` & `celery-5.3.1/celery/contrib/testing/mocks.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/contrib/testing/worker.py` & `celery-5.3.1/celery/contrib/testing/worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/events/cursesmon.py` & `celery-5.3.1/celery/events/cursesmon.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/events/dispatcher.py` & `celery-5.3.1/celery/events/dispatcher.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/events/dumper.py` & `celery-5.3.1/celery/events/dumper.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/events/event.py` & `celery-5.3.1/celery/events/event.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/events/receiver.py` & `celery-5.3.1/celery/events/receiver.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/events/snapshot.py` & `celery-5.3.1/celery/events/snapshot.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/events/state.py` & `celery-5.3.1/celery/events/state.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/exceptions.py` & `celery-5.3.1/celery/exceptions.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/fixups/django.py` & `celery-5.3.1/celery/fixups/django.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/loaders/base.py` & `celery-5.3.1/celery/loaders/base.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/loaders/default.py` & `celery-5.3.1/celery/loaders/default.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/local.py` & `celery-5.3.1/celery/local.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/platforms.py` & `celery-5.3.1/celery/platforms.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/result.py` & `celery-5.3.1/celery/result.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/schedules.py` & `celery-5.3.1/celery/schedules.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/security/__init__.py` & `celery-5.3.1/celery/security/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/security/certificate.py` & `celery-5.3.1/celery/security/certificate.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/security/key.py` & `celery-5.3.1/celery/security/key.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/security/serialization.py` & `celery-5.3.1/celery/security/serialization.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/security/utils.py` & `celery-5.3.1/celery/security/utils.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/signals.py` & `celery-5.3.1/celery/signals.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/states.py` & `celery-5.3.1/celery/states.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/utils/__init__.py` & `celery-5.3.1/celery/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/utils/abstract.py` & `celery-5.3.1/celery/utils/abstract.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/utils/collections.py` & `celery-5.3.1/celery/utils/collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,24 +202,25 @@
 class ChainMap(MutableMapping):
     """Key lookup on a sequence of maps."""
 
     key_t = None
     changes = None
     defaults = None
     maps = None
-    _observers = []
+    _observers = ()
 
     def __init__(self, *maps, **kwargs):
         # type: (*Mapping, **Any) -> None
         maps = list(maps or [{}])
         self.__dict__.update(
             key_t=kwargs.get('key_t'),
             maps=maps,
             changes=maps[0],
             defaults=maps[1:],
+            _observers=[],
         )
 
     def add_defaults(self, d):
         # type: (Mapping) -> None
         d = force_mapping(d)
         self.defaults.insert(0, d)
         self.maps.insert(1, d)
```

### Comparing `celery-5.3.0rc2/celery/utils/debug.py` & `celery-5.3.1/celery/utils/debug.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/utils/deprecated.py` & `celery-5.3.1/celery/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/utils/dispatch/signal.py` & `celery-5.3.1/celery/utils/dispatch/signal.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/utils/functional.py` & `celery-5.3.1/celery/utils/functional.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/utils/graph.py` & `celery-5.3.1/celery/utils/graph.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/utils/imports.py` & `celery-5.3.1/celery/utils/imports.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/utils/iso8601.py` & `celery-5.3.1/celery/utils/iso8601.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/utils/log.py` & `celery-5.3.1/celery/utils/log.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/utils/nodenames.py` & `celery-5.3.1/celery/utils/nodenames.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/utils/objects.py` & `celery-5.3.1/celery/utils/objects.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/utils/saferepr.py` & `celery-5.3.1/celery/utils/saferepr.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/utils/serialization.py` & `celery-5.3.1/celery/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/utils/static/celery_128.png` & `celery-5.3.1/celery/utils/static/celery_128.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/utils/sysinfo.py` & `celery-5.3.1/celery/utils/sysinfo.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/utils/term.py` & `celery-5.3.1/celery/utils/term.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/utils/text.py` & `celery-5.3.1/celery/utils/text.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/utils/threads.py` & `celery-5.3.1/celery/utils/threads.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/utils/time.py` & `celery-5.3.1/celery/utils/time.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/utils/timer2.py` & `celery-5.3.1/celery/utils/timer2.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/worker/autoscale.py` & `celery-5.3.1/celery/worker/autoscale.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/worker/components.py` & `celery-5.3.1/celery/worker/components.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/worker/consumer/agent.py` & `celery-5.3.1/celery/worker/consumer/agent.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/worker/consumer/connection.py` & `celery-5.3.1/celery/worker/consumer/connection.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/worker/consumer/consumer.py` & `celery-5.3.1/celery/worker/consumer/consumer.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/worker/consumer/control.py` & `celery-5.3.1/celery/worker/consumer/control.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/worker/consumer/events.py` & `celery-5.3.1/celery/worker/consumer/events.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/worker/consumer/gossip.py` & `celery-5.3.1/celery/worker/consumer/gossip.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/worker/consumer/heart.py` & `celery-5.3.1/celery/worker/consumer/heart.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/worker/consumer/mingle.py` & `celery-5.3.1/celery/worker/consumer/mingle.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/worker/consumer/tasks.py` & `celery-5.3.1/celery/worker/consumer/tasks.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/worker/control.py` & `celery-5.3.1/celery/worker/control.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/worker/heartbeat.py` & `celery-5.3.1/celery/worker/heartbeat.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/worker/loops.py` & `celery-5.3.1/celery/worker/loops.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/worker/pidbox.py` & `celery-5.3.1/celery/worker/pidbox.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/worker/request.py` & `celery-5.3.1/celery/worker/request.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/worker/state.py` & `celery-5.3.1/celery/worker/state.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/worker/strategy.py` & `celery-5.3.1/celery/worker/strategy.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery/worker/worker.py` & `celery-5.3.1/celery/worker/worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/celery.egg-info/PKG-INFO` & `celery-5.3.1/celery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celery
-Version: 5.3.0rc2
+Version: 5.3.1
 Summary: Distributed Task Queue.
 Home-page: https://docs.celeryq.dev/
 Author: Ask Solem
 Author-email: auvipy@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.celeryq.dev/en/stable/
 Project-URL: Changelog, https://docs.celeryq.dev/en/stable/changelog.html
@@ -19,18 +19,19 @@
 Classifier: Topic :: Software Development :: Object Brokering
 Classifier: Framework :: Celery
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: arangodb
 Provides-Extra: auth
 Provides-Extra: azureblockblob
 Provides-Extra: brotli
 Provides-Extra: cassandra
 Provides-Extra: consul
 Provides-Extra: cosmosdbsql
@@ -60,15 +61,15 @@
 Provides-Extra: zstd
 License-File: LICENSE
 
 .. image:: https://docs.celeryq.dev/en/latest/_images/celery-banner-small.png
 
 |build-status| |coverage| |license| |wheel| |semgrep| |pyversion| |pyimp| |ocbackerbadge| |ocsponsorbadge|
 
-:Version: 5.3.0rc2 (dawn-chorus)
+:Version: 5.3.1 (emerald-rush)
 :Web: https://docs.celeryq.dev/en/stable/index.html
 :Download: https://pypi.org/project/celery/
 :Source: https://github.com/celery/celery/
 :Keywords: task, queue, job, async, rabbitmq, amqp, redis,
   python, distributed, actors
 
 Donations
@@ -116,48 +117,49 @@
 .. _`gocelery`: https://github.com/gocelery/gocelery
 .. _gopher-celery: https://github.com/marselester/gopher-celery
 .. _rusty-celery: https://github.com/rusty-celery/rusty-celery
 
 What do I need?
 ===============
 
-Celery version 5.3.0a1 runs on,
+Celery version 5.3.1 runs on,
 
-- Python (3.8, 3.9, 3.10)
+- Python (3.8, 3.9, 3.10, 3.11)
 - PyPy3.8+ (v7.3.11+)
 
 
-This is the version of celery which will support Python 3.7 or newer.
+This is the version of celery which will support Python 3.8 or newer.
 
 If you're running an older version of Python, you need to be running
 an older version of Celery:
 
+- Python 3.7: Celery 5.2 or earlier.
 - Python 3.6: Celery 5.1 or earlier.
 - Python 2.7: Celery 4.x series.
 - Python 2.6: Celery series 3.1 or earlier.
 - Python 2.5: Celery series 3.0 or earlier.
 - Python 2.4: Celery series 2.2 or earlier.
 
 Celery is a project with minimal funding,
-so we don't support Microsoft Windows.
+so we don't support Microsoft Windows but it should be working.
 Please don't open any issues related to that platform.
 
 *Celery* is usually used with a message broker to send and receive messages.
 The RabbitMQ, Redis transports are feature complete,
 but there's also experimental support for a myriad of other solutions, including
 using SQLite for local development.
 
 *Celery* can run on a single machine, on multiple machines, or even
 across datacenters.
 
 Get Started
 ===========
 
 If this is the first time you're trying to use Celery, or you're
-new to Celery v5.3.0a1 coming from previous versions then you should read our
+new to Celery v5.3.1 coming from previous versions then you should read our
 getting started tutorials:
 
 - `First steps with Celery`_
 
     Tutorial teaching you the bare minimum needed to get started with Celery.
 
 - `Next steps`_
@@ -317,17 +319,17 @@
 You can specify these in your requirements or on the ``pip``
 command-line by using brackets. Multiple bundles can be specified by
 separating them by commas.
 
 ::
 
 
-    $ pip install "celery[amqp]"
+    $ pip install "celery[redis]"
 
-    $ pip install "celery[amqp,redis,auth,msgpack]"
+    $ pip install "celery[redis,auth,msgpack]"
 
 The following bundles are available:
 
 Serializers
 ~~~~~~~~~~~
 
 :``celery[auth]``:
```

### Comparing `celery-5.3.0rc2/celery.egg-info/SOURCES.txt` & `celery-5.3.1/celery.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
 docs/contributing.rst
 docs/copyright.rst
 docs/faq.rst
 docs/glossary.rst
 docs/index.rst
 docs/make.bat
 docs/spelling_wordlist.txt
-docs/whatsnew-5.2.rst
+docs/whatsnew-5.3.rst
 docs/_ext/celerydocs.py
 docs/_static/.keep
 docs/_templates/sidebardonations.html
 docs/django/first-steps-with-django.rst
 docs/django/index.rst
 docs/getting-started/first-steps-with-celery.rst
 docs/getting-started/index.rst
```

### Comparing `celery-5.3.0rc2/celery.egg-info/requires.txt` & `celery-5.3.1/celery.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 billiard<5.0,>=4.1.0
 click-didyoumean>=0.3.0
 click-plugins>=1.1.1
 click-repl>=0.2.0
 click<9.0,>=8.1.2
-kombu<6.0,>=5.3.0rc2
+kombu<6.0,>=5.3.1
 python-dateutil>=2.8.2
 tzdata>=2022.7
 vine<6.0,>=5.0.0
 
 [:python_version < "3.8"]
 importlib-metadata>=3.6
 
 [:python_version < "3.9"]
 backports.zoneinfo>=0.2.1
 
 [arangodb]
 pyArango>=2.0.1
 
 [auth]
-cryptography==40.0.2
+cryptography==41.0.1
 
 [azureblockblob]
 azure-storage-blob>=12.15.0
 
 [brotli]
 
 [brotli:platform_python_implementation == "CPython"]
@@ -48,29 +48,31 @@
 [couchdb]
 pycouchdb==1.14.2
 
 [django]
 Django>=2.2.28
 
 [dynamodb]
-boto3>=1.22.2
+boto3>=1.26.143
 
 [elasticsearch]
 elasticsearch<8.0
 
 [eventlet]
 
 [eventlet:python_version < "3.10"]
 eventlet>=0.32.0
 
 [gevent]
 gevent>=1.5.0
 
 [librabbitmq]
-librabbitmq>=1.5.0
+
+[librabbitmq:python_version < "3.11"]
+librabbitmq>=2.0.0
 
 [memcache]
 
 [memcache:platform_system != "Windows"]
 pylibmc==1.6.3
 
 [mongodb]
@@ -79,38 +81,45 @@
 [msgpack]
 msgpack==1.0.5
 
 [pymemcache]
 python-memcached==1.59
 
 [pyro]
-pyro4
+
+[pyro:python_version < "3.11"]
+pyro4==4.82
 
 [pytest]
 pytest-celery==0.0.0
 
 [redis]
-redis>=4.5.2
+redis!=4.5.5,>=4.5.2
 
 [s3]
-boto3>=1.26.139
+boto3>=1.26.143
 
 [slmq]
 softlayer_messaging>=1.0.3
 
 [solar]
 
 [solar:platform_python_implementation != "PyPy"]
 ephem==4.1.4
 
 [sqlalchemy]
 sqlalchemy<2.1,>=1.4.48
 
 [sqs]
-kombu[sqs]>=5.3.0rc2
+boto3>=1.26.143
+kombu[sqs]>=5.3.0
+urllib3>=1.26.16
+
+[sqs:sys_platform != "win32" and platform_python_implementation == "CPython"]
+pycurl>=7.43.0.5
 
 [tblib]
 
 [tblib:python_version < "3.8.0"]
 tblib>=1.3.0
 
 [tblib:python_version >= "3.8.0"]
```

### Comparing `celery-5.3.0rc2/docs/AUTHORS.txt` & `celery-5.3.1/docs/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/Makefile` & `celery-5.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/_ext/celerydocs.py` & `celery-5.3.1/docs/_ext/celerydocs.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/community.rst` & `celery-5.3.1/docs/community.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/conf.py` & `celery-5.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/copyright.rst` & `celery-5.3.1/docs/copyright.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/django/first-steps-with-django.rst` & `celery-5.3.1/docs/django/first-steps-with-django.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     Django. You'll use the same API as non-Django users so you're recommended
     to read the :ref:`first-steps` tutorial
     first and come back to this tutorial. When you have a working example you can
     continue to the :ref:`next-steps` guide.
 
 .. note::
 
-    Celery 5.0.x supports Django 1.11 LTS or newer versions. Please use Celery 4.4.x
-    for versions older than Django 1.11.
+    Celery 5.3.x supports Django 2.2 LTS or newer versions.
+    Please use Celery 5.2.x for versions older than Django 2.2 or Celery 4.4.x if your Django version is older than 1.11.
 
 To use Celery with your Django project you must first define
 an instance of the Celery library (called an "app")
 
 If you have a modern Django project layout like::
 
     - proj/
```

### Comparing `celery-5.3.0rc2/docs/faq.rst` & `celery-5.3.1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/getting-started/backends-and-brokers/index.rst` & `celery-5.3.1/docs/getting-started/backends-and-brokers/index.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/getting-started/backends-and-brokers/rabbitmq.rst` & `celery-5.3.1/docs/getting-started/backends-and-brokers/rabbitmq.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/getting-started/backends-and-brokers/redis.rst` & `celery-5.3.1/docs/getting-started/backends-and-brokers/redis.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/getting-started/backends-and-brokers/sqs.rst` & `celery-5.3.1/docs/getting-started/backends-and-brokers/sqs.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/getting-started/first-steps-with-celery.rst` & `celery-5.3.1/docs/getting-started/first-steps-with-celery.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/getting-started/introduction.rst` & `celery-5.3.1/docs/getting-started/introduction.rst`

 * *Files 1% similar despite different names*

```diff
@@ -35,18 +35,18 @@
 .. _node-celery: https://github.com/mher/node-celery
 .. _node-celery-ts: https://github.com/IBM/node-celery-ts
 
 What do I need?
 ===============
 
 .. sidebar:: Version Requirements
-    :subtitle: Celery version 5.2 runs on
+    :subtitle: Celery version 5.3 runs on
 
-    - Python ❨3.7, 3.8, 3.9, 3.10❩
-    - PyPy3.7, 3.8 ❨7.3.7❩
+    - Python ❨3.8, 3.9, 3.10, 3.11❩
+    - PyPy3.8+ ❨v7.3.11+❩
 
     Celery 4.x was the last version to support Python 2.7,
     Celery 5.x requires Python 3.6 or newer.
     Celery 5.1.x also requires Python 3.6 or newer.
     Celery 5.2.x requires Python 3.7 or newer.
```

### Comparing `celery-5.3.0rc2/docs/getting-started/next-steps.rst` & `celery-5.3.1/docs/getting-started/next-steps.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/glossary.rst` & `celery-5.3.1/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/changelog-1.0.rst` & `celery-5.3.1/docs/history/changelog-1.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/changelog-2.0.rst` & `celery-5.3.1/docs/history/changelog-2.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/changelog-2.1.rst` & `celery-5.3.1/docs/history/changelog-2.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/changelog-2.2.rst` & `celery-5.3.1/docs/history/changelog-2.2.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/changelog-2.3.rst` & `celery-5.3.1/docs/history/changelog-2.3.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/changelog-2.4.rst` & `celery-5.3.1/docs/history/changelog-2.4.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/changelog-2.5.rst` & `celery-5.3.1/docs/history/changelog-2.5.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/changelog-3.0.rst` & `celery-5.3.1/docs/history/changelog-3.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/changelog-3.1.rst` & `celery-5.3.1/docs/history/changelog-3.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/changelog-4.0.rst` & `celery-5.3.1/docs/history/changelog-4.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/changelog-4.1.rst` & `celery-5.3.1/docs/history/changelog-4.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/changelog-4.2.rst` & `celery-5.3.1/docs/history/changelog-4.2.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/changelog-4.3.rst` & `celery-5.3.1/docs/history/changelog-4.3.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/changelog-4.4.rst` & `celery-5.3.1/docs/history/changelog-4.4.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/changelog-5.0.rst` & `celery-5.3.1/docs/history/changelog-5.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/changelog-5.1.rst` & `celery-5.3.1/docs/history/changelog-5.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/index.rst` & `celery-5.3.1/docs/history/index.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/whatsnew-2.5.rst` & `celery-5.3.1/docs/history/whatsnew-2.5.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/whatsnew-3.0.rst` & `celery-5.3.1/docs/history/whatsnew-3.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/whatsnew-3.1.rst` & `celery-5.3.1/docs/history/whatsnew-3.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/whatsnew-4.0.rst` & `celery-5.3.1/docs/history/whatsnew-4.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/whatsnew-4.1.rst` & `celery-5.3.1/docs/history/whatsnew-4.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/whatsnew-4.2.rst` & `celery-5.3.1/docs/history/whatsnew-4.2.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/whatsnew-4.3.rst` & `celery-5.3.1/docs/history/whatsnew-4.3.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/whatsnew-4.4.rst` & `celery-5.3.1/docs/history/whatsnew-4.4.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/whatsnew-5.0.rst` & `celery-5.3.1/docs/history/whatsnew-5.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/history/whatsnew-5.1.rst` & `celery-5.3.1/docs/history/whatsnew-5.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/images/celery-banner-small.png` & `celery-5.3.1/docs/images/celery-banner-small.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/images/celery-banner.png` & `celery-5.3.1/docs/images/celery-banner.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/images/celery_128.png` & `celery-5.3.1/docs/images/celery_128.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/images/celery_512.png` & `celery-5.3.1/docs/images/celery_512.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/images/celeryevshotsm.jpg` & `celery-5.3.1/docs/images/celeryevshotsm.jpg`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/images/dashboard.png` & `celery-5.3.1/docs/images/dashboard.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/images/favicon.ico` & `celery-5.3.1/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/images/monitor.png` & `celery-5.3.1/docs/images/monitor.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/images/result_graph.png` & `celery-5.3.1/docs/images/result_graph.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/images/worker_graph_full.png` & `celery-5.3.1/docs/images/worker_graph_full.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/includes/installation.txt` & `celery-5.3.1/docs/includes/installation.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/includes/introduction.txt` & `celery-5.3.1/docs/includes/introduction.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-:Version: 5.3.0rc2 (dawn-chorus)
+:Version: 5.3.1 (emerald-rush)
 :Web: https://docs.celeryq.dev/en/stable/index.html
 :Download: https://pypi.org/project/celery/
 :Source: https://github.com/celery/celery/
 :Keywords: task, queue, job, async, rabbitmq, amqp, redis,
   python, distributed, actors
 
 --
```

### Comparing `celery-5.3.0rc2/docs/includes/resources.txt` & `celery-5.3.1/docs/includes/resources.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/index.rst` & `celery-5.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/internals/app-overview.rst` & `celery-5.3.1/docs/internals/app-overview.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/internals/deprecation.rst` & `celery-5.3.1/docs/internals/deprecation.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/internals/guide.rst` & `celery-5.3.1/docs/internals/guide.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/internals/protocol.rst` & `celery-5.3.1/docs/internals/protocol.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/internals/reference/index.rst` & `celery-5.3.1/docs/internals/reference/index.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/internals/worker.rst` & `celery-5.3.1/docs/internals/worker.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/make.bat` & `celery-5.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/reference/celery.app.amqp.rst` & `celery-5.3.1/docs/reference/celery.app.amqp.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/reference/celery.rst` & `celery-5.3.1/docs/reference/celery.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/reference/celery.utils.debug.rst` & `celery-5.3.1/docs/reference/celery.utils.debug.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/reference/index.rst` & `celery-5.3.1/docs/reference/index.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/sec/CELERYSA-0001.txt` & `celery-5.3.1/docs/sec/CELERYSA-0001.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/sec/CELERYSA-0002.txt` & `celery-5.3.1/docs/sec/CELERYSA-0002.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/sec/CELERYSA-0003.txt` & `celery-5.3.1/docs/sec/CELERYSA-0003.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/spelling_wordlist.txt` & `celery-5.3.1/docs/spelling_wordlist.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/templates/readme.txt` & `celery-5.3.1/docs/templates/readme.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/tutorials/task-cookbook.rst` & `celery-5.3.1/docs/tutorials/task-cookbook.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/userguide/application.rst` & `celery-5.3.1/docs/userguide/application.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/userguide/calling.rst` & `celery-5.3.1/docs/userguide/calling.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/userguide/canvas.rst` & `celery-5.3.1/docs/userguide/canvas.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/userguide/concurrency/eventlet.rst` & `celery-5.3.1/docs/userguide/concurrency/eventlet.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/userguide/configuration.rst` & `celery-5.3.1/docs/userguide/configuration.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/userguide/daemonizing.rst` & `celery-5.3.1/docs/userguide/daemonizing.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/userguide/debugging.rst` & `celery-5.3.1/docs/userguide/debugging.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/userguide/extending.rst` & `celery-5.3.1/docs/userguide/extending.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/userguide/monitoring.rst` & `celery-5.3.1/docs/userguide/monitoring.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/userguide/optimizing.rst` & `celery-5.3.1/docs/userguide/optimizing.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/userguide/periodic-tasks.rst` & `celery-5.3.1/docs/userguide/periodic-tasks.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/userguide/routing.rst` & `celery-5.3.1/docs/userguide/routing.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/userguide/security.rst` & `celery-5.3.1/docs/userguide/security.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/userguide/signals.rst` & `celery-5.3.1/docs/userguide/signals.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/userguide/tasks.rst` & `celery-5.3.1/docs/userguide/tasks.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/userguide/testing.rst` & `celery-5.3.1/docs/userguide/testing.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/userguide/workers.rst` & `celery-5.3.1/docs/userguide/workers.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/docs/whatsnew-5.2.rst` & `celery-5.3.1/docs/whatsnew-5.3.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-.. _whatsnew-5.2:
+.. _whatsnew-5.3:
 
 =========================================
- What's new in Celery 5.2 (Dawn Chorus)
+ What's new in Celery 5.3 (Emerald Rush)
 =========================================
-:Author: Omer Katz (``omer.drow at gmail.com``)
+:Author: Asif Saif Uddin (``auvipy at gmail.com``).
 
 .. sidebar:: Change history
 
     What's new documents describe the changes in major versions,
     we also have a :ref:`changelog` that lists the changes in bugfix
     releases (0.0.x), while older series are archived under the :ref:`history`
     section.
@@ -33,45 +33,45 @@
 
 To read more about Celery you should go read the :ref:`introduction <intro>`.
 
 While this version is **mostly** backward compatible with previous versions
 it's important that you read the following section as this release
 is a new major version.
 
-This version is officially supported on CPython 3.7 & 3.8 & 3.9
-and is also supported on PyPy3.
+This version is officially supported on CPython 3.8, 3.9 & 3.10
+and is also supported on PyPy3.8+.
 
-.. _`website`: http://celeryproject.org/
+.. _`website`: https://docs.celeryq.dev/en/stable/
 
 .. topic:: Table of Contents
 
     Make sure you read the important notes before upgrading to this version.
 
 .. contents::
     :local:
     :depth: 2
 
 Preface
 =======
 
 .. note::
 
-    **This release contains fixes for two (potentially severe) memory leaks.
+    **This release contains fixes for many long standing bugs & stability issues.
     We encourage our users to upgrade to this release as soon as possible.**
 
-The 5.2.0 release is a new minor release for Celery.
+The 5.3.0 release is a new feature release for Celery.
 
 Releases in the 5.x series are codenamed after songs of `Jon Hopkins <https://en.wikipedia.org/wiki/Jon_Hopkins>`_.
-This release has been codenamed `Dawn Chorus <https://www.youtube.com/watch?v=bvsZBdo5pEk>`_.
+This release has been codenamed `Emerald Rush <https://www.youtube.com/watch?v=4sk0uDbM5lc>`_.
 
-From now on we only support Python 3.7 and above.
-We will maintain compatibility with Python 3.7 until it's
-EOL in June, 2023.
+From now on we only support Python 3.8 and above.
+We will maintain compatibility with Python 3.8 until it's
+EOL in 2024.
 
-*— Omer Katz*
+*— Asif Saif Uddin*
 
 Long Term Support Policy
 ------------------------
 
 We no longer support Celery 4.x as we don't have the resources to do so.
 If you'd like to help us, all contributions are welcome.
 
@@ -137,257 +137,213 @@
 You can use tools like `2to3 <https://docs.python.org/3.8/library/2to3.html>`_
 and `pyupgrade <https://github.com/asottile/pyupgrade>`_ to assist you with
 this effort.
 
 After the migration is done, run your test suite with Celery 4 to ensure
 nothing has been broken.
 
-Step 5: Upgrade to Celery 5.2
+Step 5: Upgrade to Celery 5.3
 -----------------------------
 
 At this point you can upgrade your workers and clients with the new version.
 
-.. _v520-important:
+.. _v530-important:
 
 Important Notes
 ===============
 
 Supported Python Versions
 -------------------------
 
 The supported Python versions are:
 
-- CPython 3.7
 - CPython 3.8
 - CPython 3.9
-- PyPy3.7 7.3 (``pypy3``)
+- CPython 3.10
+- PyPy3.8 7.3.11 (``pypy3``)
 
 Experimental support
 ~~~~~~~~~~~~~~~~~~~~
 
 Celery supports these Python versions provisionally as they are not production
 ready yet:
 
-- CPython 3.10 (currently in RC2)
+- CPython 3.11
 
-Memory Leak Fixes
------------------
+Quality Improvements and Stability Enhancements
+-----------------------------------------------
 
-Two severe memory leaks have been fixed in this version:
+Celery 5.3 focuses on elevating the overall quality and stability of the project. 
+We have dedicated significant efforts to address various bugs, enhance performance,
+and make improvements based on valuable user feedback.
+
+Better Compatibility and Upgrade Confidence
+-------------------------------------------
+
+Our goal with Celery 5.3 is to instill confidence in users who are currently 
+using Celery 4 or older versions. We want to assure you that upgrading to 
+Celery 5.3 will provide a more robust and reliable experience.
 
-* :class:`celery.result.ResultSet` no longer holds a circular reference to itself.
-* The prefork pool no longer keeps messages in its cache forever when the master
-  process disconnects from the broker.
-
-The first memory leak occurs when you use :class:`celery.result.ResultSet`.
-Each instance held a promise which provides that instance as an argument to
-the promise's callable.
-This caused a circular reference which kept the ResultSet instance in memory
-forever since the GC couldn't evict it.
-The provided argument is now a :func:`weakref.proxy` of the ResultSet's
-instance.
-The memory leak mainly occurs when you use :class:`celery.result.GroupResult`
-since it inherits from :class:`celery.result.ResultSet` which doesn't get used
-that often.
-
-The second memory leak exists since the inception of the project.
-The prefork pool maintains a cache of the jobs it executes.
-When they are complete, they are evicted from the cache.
-However, when Celery disconnects from the broker, we flush the pool
-and discard the jobs, expecting that they'll be cleared later once the worker
-acknowledges them but that has never been the case.
-Instead, these jobs remain forever in memory.
-We now discard those jobs immediately while flushing.
 
-Dropped support for Python 3.6
+Dropped support for Python 3.7
 ------------------------------
 
-Celery now requires Python 3.7 and above.
+Celery now requires Python 3.8 and above.
 
-Python 3.6 will reach EOL in December, 2021.
+Python 3.7 will reach EOL in June, 2023.
 In order to focus our efforts we have dropped support for Python 3.6 in
 this version.
 
-If you still require to run Celery using Python 3.6
-you can still use Celery 5.1.
+If you still require to run Celery using Python 3.7
+you can still use Celery 5.2.
 However we encourage you to upgrade to a supported Python version since
-no further security patches will be applied for Python 3.6 after
-the 23th of December, 2021.
+no further security patches will be applied for Python 3.7 after
+the 23th of June, 2023.
 
-Tasks
------
 
-When replacing a task with another task, we now give an indication of the
-replacing nesting level through the ``replaced_task_nesting`` header.
+Automatic re-connection on connection loss to broker
+----------------------------------------------------
+
+Unless :setting:`broker_connection_retry_on_startup` is set to False,
+Celery will automatically retry reconnecting to the broker after 
+the first connection loss. :setting:`broker_connection_retry` controls 
+whether to automatically retry reconnecting to the broker for subsequent
+reconnects.
+
+Since the message broker does not track how many tasks were already fetched 
+before the connection was lost, Celery will reduce the prefetch count by 
+the number of tasks that are currently running multiplied by 
+:setting:`worker_prefetch_multiplier`.
+The prefetch count will be gradually restored to the maximum allowed after
+each time a task that was running before the connection was lost is complete
 
-A task which was never replaced has a ``replaced_task_nesting`` value of 0.
 
 Kombu
 -----
 
-Starting from v5.2, the minimum required version is Kombu 5.2.0.
-
-Prefork Workers Pool
----------------------
-
-Now all orphaned worker processes are killed automatically when main process exits.
-
-Eventlet Workers Pool
----------------------
-
-You can now terminate running revoked tasks while using the
-Eventlet Workers Pool.
-
-Custom Task Classes
--------------------
-
-We introduced a custom handler which will be executed before the task
-is started called ``before_start``.
-
-See :ref:`custom-task-cls-app-wide` for more details.
-
-Important Notes From 5.0
-------------------------
+Starting from v5.3.0, the minimum required version is Kombu 5.3.0.
 
-Dropped support for Python 2.7 & 3.5
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Celery now requires Python 3.6 and above.
+Redis
+-----
 
-Python 2.7 has reached EOL in January 2020.
-In order to focus our efforts we have dropped support for Python 2.7 in
-this version.
+redis-py 4.5.x is the new minimum required version.
 
-In addition, Python 3.5 has reached EOL in September 2020.
-Therefore, we are also dropping support for Python 3.5.
 
-If you still require to run Celery using Python 2.7 or Python 3.5
-you can still use Celery 4.x.
-However we encourage you to upgrade to a supported Python version since
-no further security patches will be applied for Python 2.7 or
-Python 3.5.
+SQLAlchemy
+---------------------
 
-Eventlet Workers Pool
-~~~~~~~~~~~~~~~~~~~~~
+SQLAlchemy 1.4.x & 2.0.x is now supported in celery v5.3
 
-Due to `eventlet/eventlet#526 <https://github.com/eventlet/eventlet/issues/526>`_
-the minimum required version is eventlet 0.26.1.
 
-Gevent Workers Pool
-~~~~~~~~~~~~~~~~~~~
+Billiard
+-------------------
 
-Starting from v5.0, the minimum required version is gevent 1.0.0.
+Minimum required version is now 4.1.0
 
-Couchbase Result Backend
-~~~~~~~~~~~~~~~~~~~~~~~~
 
-The Couchbase result backend now uses the V3 Couchbase SDK.
+Deprecate pytz and use zoneinfo
+-------------------------------
 
-As a result, we no longer support Couchbase Server 5.x.
+A switch have been made to zoneinfo for handling timezone data instead of pytz.
 
-Also, starting from v5.0, the minimum required version
-for the database client is couchbase 3.0.0.
 
-To verify that your Couchbase Server is compatible with the V3 SDK,
-please refer to their `documentation <https://docs.couchbase.com/python-sdk/3.0/project-docs/compatibility.html>`_.
+Support for out-of-tree worker pool implementations
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Prior to version 5.3, Celery had a fixed notion of the worker pool types it supports.
+Celery v5.3.0 introduces the the possibility of an out-of-tree worker pool implementation.
+This feature ensure that the current worker pool implementations consistently call into
+BasePool._get_info(), and enhance it to report the work pool class in use via the 
+"celery inspect stats" command. For example:
 
-Riak Result Backend
-~~~~~~~~~~~~~~~~~~~
+$ celery -A ... inspect stats
+->  celery@freenas: OK
+    {
+        ...
+        "pool": {
+           ...
+            "implementation": "celery_aio_pool.pool:AsyncIOPool",
 
-The Riak result backend has been removed as the database is no longer maintained.
+It can be used as follows:
 
-The Python client only supports Python 3.6 and below which prevents us from
-supporting it and it is also unmaintained.
+    Set the environment variable CELERY_CUSTOM_WORKER_POOL to the name of
+    an implementation of :class:celery.concurrency.base.BasePool in the
+    standard Celery format of "package:class".
 
-If you are still using Riak, refrain from upgrading to Celery 5.0 while you
-migrate your application to a different database.
+    Select this pool using '--pool custom'.
 
-We apologize for the lack of notice in advance but we feel that the chance
-you'll be affected by this breaking change is minimal which is why we
-did it.
 
-AMQP Result Backend
-~~~~~~~~~~~~~~~~~~~
+Signal::``worker_before_create_process``
+----------------------------------------
 
-The AMQP result backend has been removed as it was deprecated in version 4.0.
+Dispatched in the parent process, just before new child process is created in the prefork pool.
+It can be used to clean up instances that don't behave well when forking.
 
-Removed Deprecated Modules
-~~~~~~~~~~~~~~~~~~~~~~~~~~
+.. code-block:: python
+    @signals.worker_before_create_process.connect
+    def clean_channels(**kwargs):
+        grpc_singleton.clean_channel()
 
-The `celery.utils.encoding` and the `celery.task` modules has been deprecated
-in version 4.0 and therefore are removed in 5.0.
 
-If you were using the `celery.utils.encoding` module before,
-you should import `kombu.utils.encoding` instead.
+Setting::``beat_cron_starting_deadline``
+----------------------------------------
 
-If you were using the `celery.task` module before, you should import directly
-from the `celery` module instead.
+When using cron, the number of seconds :mod:`~celery.bin.beat` can look back
+when deciding whether a cron schedule is due. When set to `None`, cronjobs that
+are past due will always run immediately.
 
-`azure-servicebus` 7.0.0 is now required
-----------------------------------------
 
-Given the SDK changes between 0.50.0 and 7.0.0 Kombu deprecates support for
-older `azure-servicebus` versions.
+Redis result backend Global keyprefix
+-------------------------------------
 
-.. _v520-news:
+The global key prefix will be prepended to all keys used for the result backend,
+which can be useful when a redis database is shared by different users.
+By default, no prefix is prepended.
 
-Bug: Pymongo 3.12.1 is not compatible with Celery 5.2
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+To configure the global keyprefix for the Redis result backend, use the 
+``global_keyprefix`` key under :setting:`result_backend_transport_options`:
 
-For now we are limiting Pymongo version, only allowing for versions between 3.3.0 and 3.12.0.
 
-This will be fixed in the next patch.
+.. code-block:: python
+    app.conf.result_backend_transport_options = {
+        'global_keyprefix': 'my_prefix_'
+    }
 
-News
-====
 
-Support for invoking chords of unregistered tasks
--------------------------------------------------
+Django
+------
 
-Previously if you attempted to publish a chord
-while providing a signature which wasn't registered in the Celery app publishing
-the chord as the body of the chord, an :exc:`celery.exceptions.NotRegistered`
-exception would be raised.
+Minimum django version is bumped to v2.2.28.
+Also added --skip-checks flag to bypass django core checks.
 
-From now on, you can publish these sort of chords and they would be executed
-correctly:
 
-.. code-block:: python
+Make default worker state limits configurable
+---------------------------------------------
 
-    # movies.task.publish_movie is registered in the current app
-    movie_task = celery_app.signature('movies.task.publish_movie', task_id=str(uuid.uuid4()), immutable=True)
-    # news.task.publish_news is *not* registered in the current app
-    news_task = celery_app.signature('news.task.publish_news', task_id=str(uuid.uuid4()), immutable=True)
-
-    my_chord = chain(movie_task,
-                     group(movie_task.set(task_id=str(uuid.uuid4())),
-                           movie_task.set(task_id=str(uuid.uuid4()))),
-                     news_task)
-    my_chord.apply_async()  # <-- No longer raises an exception
+Previously, `REVOKES_MAX`, `REVOKE_EXPIRES`, `SUCCESSFUL_MAX` and
+`SUCCESSFUL_EXPIRES` were hardcoded in `celery.worker.state`. This 
+version introduces `CELERY_WORKER_` prefixed environment variables 
+with the same names that allow you to customize these values should
+you need to.
 
-Consul Result Backend
----------------------
 
-We now create a new client per request to Consul to avoid a bug in the Consul
-client.
+Canvas stamping
+---------------
 
-The Consul Result Backend now accepts a new
-:setting:`result_backend_transport_options` key: ``one_client``.
-You can opt out of this behavior by setting ``one_client`` to True.
+The goal of the Stamping API is to give an ability to label the signature 
+and its components for debugging information purposes. For example, when 
+the canvas is a complex structure, it may be necessary to label some or 
+all elements of the formed structure. The complexity increases even more 
+when nested groups are rolled-out or chain elements are replaced. In such 
+cases, it may be necessary to understand which group an element is a part 
+of or on what nested level it is. This requires a mechanism that traverses 
+the canvas elements and marks them with specific metadata. The stamping API 
+allows doing that based on the Visitor pattern.
 
-Please refer to the documentation of the backend if you're using the Consul
-backend to find out which behavior suites you.
 
-Filesystem Result Backend
--------------------------
+Known Issues
+------------
+Canvas header stamping has issues in a hybrid Celery 4.x. & Celery 5.3.x 
+environment and is not safe for production use at the moment.
 
-We now cleanup expired task results while using the
-filesystem result backend as most result backends do.
 
-ArangoDB Result Backend
------------------------
 
-You can now check the validity of the CA certificate while making
-a TLS connection to ArangoDB result backend.
 
-If you'd like to do so, set the ``verify`` key in the
-:setting:`arangodb_backend_settings` dictionary to ``True``.
```

### Comparing `celery-5.3.0rc2/examples/app/myapp.py` & `celery-5.3.1/examples/app/myapp.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/examples/celery_http_gateway/README.rst` & `celery-5.3.1/examples/celery_http_gateway/README.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/examples/celery_http_gateway/settings.py` & `celery-5.3.1/examples/celery_http_gateway/settings.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/examples/celery_http_gateway/urls.py` & `celery-5.3.1/examples/celery_http_gateway/urls.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/examples/django/README.rst` & `celery-5.3.1/examples/django/README.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/examples/django/proj/celery.py` & `celery-5.3.1/examples/django/proj/celery.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/examples/django/proj/settings.py` & `celery-5.3.1/examples/django/proj/settings.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/examples/django/proj/urls.py` & `celery-5.3.1/examples/django/proj/urls.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/examples/django/proj/wsgi.py` & `celery-5.3.1/examples/django/proj/wsgi.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/examples/eventlet/README.rst` & `celery-5.3.1/examples/eventlet/README.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/examples/eventlet/bulk_task_producer.py` & `celery-5.3.1/examples/eventlet/bulk_task_producer.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/examples/eventlet/webcrawler.py` & `celery-5.3.1/examples/eventlet/webcrawler.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/examples/next-steps/setup.py` & `celery-5.3.1/examples/next-steps/setup.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/examples/periodic-tasks/myapp.py` & `celery-5.3.1/examples/periodic-tasks/myapp.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/examples/resultgraph/tasks.py` & `celery-5.3.1/examples/resultgraph/tasks.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/examples/security/mysecureapp.py` & `celery-5.3.1/examples/security/mysecureapp.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/examples/security/ssl/worker.key` & `celery-5.3.1/examples/security/ssl/worker.key`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/examples/security/ssl/worker.pem` & `celery-5.3.1/examples/security/ssl/worker.pem`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/examples/stamping/examples.py` & `celery-5.3.1/examples/stamping/examples.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/examples/stamping/myapp.py` & `celery-5.3.1/examples/stamping/myapp.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/examples/stamping/revoke_example.py` & `celery-5.3.1/examples/stamping/revoke_example.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/examples/stamping/tasks.py` & `celery-5.3.1/examples/stamping/tasks.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/examples/stamping/visitors.py` & `celery-5.3.1/examples/stamping/visitors.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/extra/bash-completion/celery.bash` & `celery-5.3.1/extra/bash-completion/celery.bash`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/extra/generic-init.d/celerybeat` & `celery-5.3.1/extra/generic-init.d/celerybeat`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/extra/generic-init.d/celeryd` & `celery-5.3.1/extra/generic-init.d/celeryd`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/extra/macOS/org.celeryq.beat.plist` & `celery-5.3.1/extra/macOS/org.celeryq.beat.plist`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/extra/macOS/org.celeryq.worker.plist` & `celery-5.3.1/extra/macOS/org.celeryq.worker.plist`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/extra/supervisord/celerybeat.conf` & `celery-5.3.1/extra/supervisord/celerybeat.conf`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/extra/supervisord/celeryd.conf` & `celery-5.3.1/extra/supervisord/celeryd.conf`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/extra/supervisord/supervisord.conf` & `celery-5.3.1/extra/supervisord/supervisord.conf`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/extra/systemd/celery.service` & `celery-5.3.1/extra/systemd/celery.service`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/extra/zsh-completion/celery.zsh` & `celery-5.3.1/extra/zsh-completion/celery.zsh`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/pyproject.toml` & `celery-5.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/requirements/README.rst` & `celery-5.3.1/requirements/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,16 @@
 
 
 Index
 =====
 
 * :file:`requirements/default.txt`
 
-    Default requirements for Python 3.7+.
+    Default requirements for Python 3.8+.
 
-* :file:`requirements/jython.txt`
-
-    Extra requirements needed to run on Jython 2.5
 
 * :file:`requirements/security.txt`
 
     Extra requirements needed to use the message signing serializer,
     see the Security Guide.
 
 * :file:`requirements/test.txt`
@@ -25,15 +22,15 @@
 
 * :file:`requirements/test-ci-base.txt`
 
     Extra test requirements required by the CI suite (Tox).
 
 * :file:`requirements/test-ci-default.txt`
 
-    Extra test requirements required for Python 3.7 by the CI suite (Tox).
+    Extra test requirements required for Python 3.8 by the CI suite (Tox).
 
 * :file:`requirements/test-integration.txt`
 
     Extra requirements needed when running the integration test suite.
 
 * :file:`requirements/doc.txt`
```

### Comparing `celery-5.3.0rc2/requirements/test-ci-default.txt` & `celery-5.3.1/requirements/test-ci-default.txt`

 * *Files 23% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 -r extras/consul.txt
 -r extras/cosmosdbsql.txt
 -r extras/cassandra.txt
 -r extras/azureblockblob.txt
 git+https://github.com/celery/kombu.git
 
 # SQS dependencies other than boto
-pycurl==7.43.0.5
+pycurl>=7.43.0.5; sys_platform != 'win32' and platform_python_implementation=="CPython"
+
```

### Comparing `celery-5.3.0rc2/setup.py` & `celery-5.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     keywords=meta['keywords'],
     author=meta['author'],
     author_email=meta['contact'],
     url=meta['homepage'],
     license='BSD-3-Clause',
     platforms=['any'],
     install_requires=install_requires(),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     tests_require=reqs('test.txt'),
     extras_require=extras_require(),
     entry_points={
         'console_scripts': [
             'celery = celery.__main__:main',
         ]
     },
@@ -168,12 +168,13 @@
         "Topic :: Software Development :: Object Brokering",
         "Framework :: Celery",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Operating System :: OS Independent"
     ]
 )
```

### Comparing `celery-5.3.0rc2/t/benchmarks/bench_worker.py` & `celery-5.3.1/t/benchmarks/bench_worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/integration/conftest.py` & `celery-5.3.1/t/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/integration/tasks.py` & `celery-5.3.1/t/integration/tasks.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/integration/test_backend.py` & `celery-5.3.1/t/integration/test_backend.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/integration/test_canvas.py` & `celery-5.3.1/t/integration/test_canvas.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/integration/test_inspect.py` & `celery-5.3.1/t/integration/test_inspect.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/integration/test_security.py` & `celery-5.3.1/t/integration/test_security.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/integration/test_tasks.py` & `celery-5.3.1/t/integration/test_tasks.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/integration/test_worker.py` & `celery-5.3.1/t/integration/test_worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/app/test_amqp.py` & `celery-5.3.1/t/unit/app/test_amqp.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/app/test_annotations.py` & `celery-5.3.1/t/unit/app/test_annotations.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/app/test_app.py` & `celery-5.3.1/t/unit/app/test_app.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/app/test_backends.py` & `celery-5.3.1/t/unit/app/test_backends.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/app/test_beat.py` & `celery-5.3.1/t/unit/app/test_beat.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/app/test_builtins.py` & `celery-5.3.1/t/unit/app/test_builtins.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/app/test_control.py` & `celery-5.3.1/t/unit/app/test_control.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/app/test_defaults.py` & `celery-5.3.1/t/unit/app/test_defaults.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/app/test_exceptions.py` & `celery-5.3.1/t/unit/app/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/app/test_loaders.py` & `celery-5.3.1/t/unit/app/test_loaders.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/app/test_log.py` & `celery-5.3.1/t/unit/app/test_log.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/app/test_registry.py` & `celery-5.3.1/t/unit/app/test_registry.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/app/test_routes.py` & `celery-5.3.1/t/unit/app/test_routes.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/app/test_schedules.py` & `celery-5.3.1/t/unit/app/test_schedules.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/app/test_utils.py` & `celery-5.3.1/t/unit/app/test_utils.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/apps/test_multi.py` & `celery-5.3.1/t/unit/apps/test_multi.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/backends/test_arangodb.py` & `celery-5.3.1/t/unit/backends/test_arangodb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/backends/test_asynchronous.py` & `celery-5.3.1/t/unit/backends/test_asynchronous.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/backends/test_azureblockblob.py` & `celery-5.3.1/t/unit/backends/test_azureblockblob.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/backends/test_base.py` & `celery-5.3.1/t/unit/backends/test_base.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/backends/test_cache.py` & `celery-5.3.1/t/unit/backends/test_cache.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/backends/test_cassandra.py` & `celery-5.3.1/t/unit/backends/test_cassandra.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/backends/test_consul.py` & `celery-5.3.1/t/unit/backends/test_consul.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/backends/test_cosmosdbsql.py` & `celery-5.3.1/t/unit/backends/test_cosmosdbsql.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/backends/test_couchbase.py` & `celery-5.3.1/t/unit/backends/test_couchbase.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/backends/test_couchdb.py` & `celery-5.3.1/t/unit/backends/test_couchdb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/backends/test_database.py` & `celery-5.3.1/t/unit/backends/test_database.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/backends/test_dynamodb.py` & `celery-5.3.1/t/unit/backends/test_dynamodb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/backends/test_elasticsearch.py` & `celery-5.3.1/t/unit/backends/test_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/backends/test_filesystem.py` & `celery-5.3.1/t/unit/backends/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/backends/test_mongodb.py` & `celery-5.3.1/t/unit/backends/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/backends/test_redis.py` & `celery-5.3.1/t/unit/backends/test_redis.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/backends/test_rpc.py` & `celery-5.3.1/t/unit/backends/test_rpc.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/backends/test_s3.py` & `celery-5.3.1/t/unit/backends/test_s3.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/bin/test_beat.py` & `celery-5.3.1/t/unit/bin/test_beat.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/bin/test_worker.py` & `celery-5.3.1/t/unit/bin/test_worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/concurrency/test_concurrency.py` & `celery-5.3.1/t/unit/concurrency/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/concurrency/test_eventlet.py` & `celery-5.3.1/t/unit/concurrency/test_eventlet.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/concurrency/test_gevent.py` & `celery-5.3.1/t/unit/concurrency/test_gevent.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/concurrency/test_pool.py` & `celery-5.3.1/t/unit/concurrency/test_pool.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/concurrency/test_prefork.py` & `celery-5.3.1/t/unit/concurrency/test_prefork.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/concurrency/test_solo.py` & `celery-5.3.1/t/unit/concurrency/test_solo.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/concurrency/test_thread.py` & `celery-5.3.1/t/unit/concurrency/test_thread.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/conftest.py` & `celery-5.3.1/t/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/contrib/test_abortable.py` & `celery-5.3.1/t/unit/contrib/test_abortable.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/contrib/test_migrate.py` & `celery-5.3.1/t/unit/contrib/test_migrate.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/contrib/test_pytest.py` & `celery-5.3.1/t/unit/contrib/test_pytest.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/contrib/test_rdb.py` & `celery-5.3.1/t/unit/contrib/test_rdb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/contrib/test_sphinx.py` & `celery-5.3.1/t/unit/contrib/test_sphinx.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/contrib/test_worker.py` & `celery-5.3.1/t/unit/contrib/test_worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/events/test_cursesmon.py` & `celery-5.3.1/t/unit/events/test_cursesmon.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/events/test_events.py` & `celery-5.3.1/t/unit/events/test_events.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/events/test_snapshot.py` & `celery-5.3.1/t/unit/events/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/events/test_state.py` & `celery-5.3.1/t/unit/events/test_state.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/fixups/test_django.py` & `celery-5.3.1/t/unit/fixups/test_django.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/security/__init__.py` & `celery-5.3.1/t/unit/security/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/security/test_certificate.py` & `celery-5.3.1/t/unit/security/test_certificate.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/security/test_key.py` & `celery-5.3.1/t/unit/security/test_key.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/security/test_security.py` & `celery-5.3.1/t/unit/security/test_security.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/security/test_serialization.py` & `celery-5.3.1/t/unit/security/test_serialization.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/tasks/test_canvas.py` & `celery-5.3.1/t/unit/tasks/test_canvas.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/tasks/test_chord.py` & `celery-5.3.1/t/unit/tasks/test_chord.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/tasks/test_context.py` & `celery-5.3.1/t/unit/tasks/test_context.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/tasks/test_result.py` & `celery-5.3.1/t/unit/tasks/test_result.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/tasks/test_stamping.py` & `celery-5.3.1/t/unit/tasks/test_stamping.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/tasks/test_states.py` & `celery-5.3.1/t/unit/tasks/test_states.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/tasks/test_tasks.py` & `celery-5.3.1/t/unit/tasks/test_tasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -244,36 +244,14 @@
                        retry_kwargs={'max_retries': 5}, shared=False)
         def autoretry_arith_task(self, a, b):
             self.iterations += 1
             return a / b
 
         self.autoretry_arith_task = autoretry_arith_task
 
-        @self.app.task(bind=True, autoretry_for=(HTTPError,),
-                       retry_backoff=True, shared=False)
-        def autoretry_backoff_task(self, url):
-            self.iterations += 1
-            if "error" in url:
-                fp = tempfile.TemporaryFile()
-                raise HTTPError(url, '500', 'Error', '', fp)
-            return url
-
-        self.autoretry_backoff_task = autoretry_backoff_task
-
-        @self.app.task(bind=True, autoretry_for=(HTTPError,),
-                       retry_backoff=True, retry_jitter=True, shared=False)
-        def autoretry_backoff_jitter_task(self, url):
-            self.iterations += 1
-            if "error" in url:
-                fp = tempfile.TemporaryFile()
-                raise HTTPError(url, '500', 'Error', '', fp)
-            return url
-
-        self.autoretry_backoff_jitter_task = autoretry_backoff_jitter_task
-
         @self.app.task(bind=True, base=TaskWithRetry, shared=False)
         def autoretry_for_from_base_task(self, a, b):
             self.iterations += 1
             return a + b
 
         self.autoretry_for_from_base_task = autoretry_for_from_base_task
 
@@ -612,43 +590,80 @@
 
     def test_autoretry_arith(self):
         self.autoretry_arith_task.max_retries = 3
         self.autoretry_arith_task.iterations = 0
         self.autoretry_arith_task.apply((1, 0))
         assert self.autoretry_arith_task.iterations == 1
 
-    @patch('random.randrange', side_effect=lambda i: i - 1)
-    def test_autoretry_backoff(self, randrange):
-        task = self.autoretry_backoff_task
-        task.max_retries = 3
+    @pytest.mark.parametrize(
+        'retry_backoff, expected_countdowns',
+        [
+            (False, [None, None, None, None]),
+            (0, [None, None, None, None]),
+            (0.0, [None, None, None, None]),
+            (True, [1, 2, 4, 8]),
+            (-1, [1, 2, 4, 8]),
+            (0.1, [1, 2, 4, 8]),
+            (1, [1, 2, 4, 8]),
+            (1.9, [1, 2, 4, 8]),
+            (2, [2, 4, 8, 16]),
+        ],
+    )
+    def test_autoretry_backoff(self, retry_backoff, expected_countdowns):
+        @self.app.task(bind=True, shared=False, autoretry_for=(ZeroDivisionError,),
+                       retry_backoff=retry_backoff, retry_jitter=False, max_retries=3)
+        def task(self_, x, y):
+            self_.iterations += 1
+            return x / y
+
         task.iterations = 0
 
         with patch.object(task, 'retry', wraps=task.retry) as fake_retry:
-            task.apply(("http://httpbin.org/error",))
+            task.apply((1, 0))
 
         assert task.iterations == 4
         retry_call_countdowns = [
-            call_[1]['countdown'] for call_ in fake_retry.call_args_list
+            call_[1].get('countdown') for call_ in fake_retry.call_args_list
         ]
-        assert retry_call_countdowns == [1, 2, 4, 8]
+        assert retry_call_countdowns == expected_countdowns
 
+    @pytest.mark.parametrize(
+        'retry_backoff, expected_countdowns',
+        [
+            (False, [None, None, None, None]),
+            (0, [None, None, None, None]),
+            (0.0, [None, None, None, None]),
+            (True, [0, 1, 3, 7]),
+            (-1, [0, 1, 3, 7]),
+            (0.1, [0, 1, 3, 7]),
+            (1, [0, 1, 3, 7]),
+            (1.9, [0, 1, 3, 7]),
+            (2, [1, 3, 7, 15]),
+        ],
+    )
     @patch('random.randrange', side_effect=lambda i: i - 2)
-    def test_autoretry_backoff_jitter(self, randrange):
-        task = self.autoretry_backoff_jitter_task
-        task.max_retries = 3
+    def test_autoretry_backoff_jitter(self, randrange, retry_backoff, expected_countdowns):
+        @self.app.task(bind=True, shared=False, autoretry_for=(HTTPError,),
+                       retry_backoff=retry_backoff, retry_jitter=True, max_retries=3)
+        def task(self_, url):
+            self_.iterations += 1
+            if "error" in url:
+                fp = tempfile.TemporaryFile()
+                raise HTTPError(url, '500', 'Error', '', fp)
+
         task.iterations = 0
 
         with patch.object(task, 'retry', wraps=task.retry) as fake_retry:
             task.apply(("http://httpbin.org/error",))
 
         assert task.iterations == 4
         retry_call_countdowns = [
-            call_[1]['countdown'] for call_ in fake_retry.call_args_list
+            call_[1].get('countdown') for call_ in fake_retry.call_args_list
         ]
-        assert retry_call_countdowns == [0, 1, 3, 7]
+        assert retry_call_countdowns == expected_countdowns
 
     def test_autoretry_for_from_base(self):
         self.autoretry_for_from_base_task.iterations = 0
         self.autoretry_for_from_base_task.apply((1, "a"))
         assert self.autoretry_for_from_base_task.iterations == 6
 
     def test_override_autoretry_for_from_base(self):
@@ -740,34 +755,55 @@
         self.app.conf.timezone = 'US/Eastern'
         self.autoretry_task.iterations = 0
         self.autoretry_task.default_retry_delay = 2
 
         self.autoretry_task.apply((1, 0))
         assert self.autoretry_task.iterations == 6
 
-    def test_autoretry_class_based_task(self):
+    @pytest.mark.parametrize(
+        'backoff_value, expected_countdowns',
+        [
+            (False, [None, None, None]),
+            (0, [None, None, None]),
+            (0.0, [None, None, None]),
+            (True, [1, 2, 4]),
+            (-1, [1, 2, 4]),
+            (0.1, [1, 2, 4]),
+            (1, [1, 2, 4]),
+            (1.9, [1, 2, 4]),
+            (2, [2, 4, 8]),
+        ],
+    )
+    def test_autoretry_class_based_task(self, backoff_value, expected_countdowns):
         class ClassBasedAutoRetryTask(Task):
             name = 'ClassBasedAutoRetryTask'
             autoretry_for = (ZeroDivisionError,)
-            retry_kwargs = {'max_retries': 5}
-            retry_backoff = True
+            retry_kwargs = {'max_retries': 2}
+            retry_backoff = backoff_value
             retry_backoff_max = 700
             retry_jitter = False
             iterations = 0
             _app = self.app
 
             def run(self, x, y):
                 self.iterations += 1
                 return x / y
 
         task = ClassBasedAutoRetryTask()
         self.app.tasks.register(task)
         task.iterations = 0
-        task.apply([1, 0])
-        assert task.iterations == 6
+
+        with patch.object(task, 'retry', wraps=task.retry) as fake_retry:
+            task.apply((1, 0))
+
+        assert task.iterations == 3
+        retry_call_countdowns = [
+            call_[1].get('countdown') for call_ in fake_retry.call_args_list
+        ]
+        assert retry_call_countdowns == expected_countdowns
 
 
 class test_canvas_utils(TasksCase):
 
     def test_si(self):
         assert self.retry_task.si()
         assert self.retry_task.si().immutable
```

### Comparing `celery-5.3.0rc2/t/unit/tasks/test_trace.py` & `celery-5.3.1/t/unit/tasks/test_trace.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/test_canvas.py` & `celery-5.3.1/t/unit/test_canvas.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/utils/test_collections.py` & `celery-5.3.1/t/unit/utils/test_collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import pickle
 from collections.abc import Mapping
 from itertools import count
 from time import monotonic
+from unittest.mock import Mock
 
 import pytest
 from billiard.einfo import ExceptionInfo
 
 import t.skip
-from celery.utils.collections import (AttributeDict, BufferMap, ConfigurationView, DictAttribute, LimitedSet,
-                                      Messagebuffer)
+from celery.utils.collections import (AttributeDict, BufferMap, ChainMap, ConfigurationView, DictAttribute,
+                                      LimitedSet, Messagebuffer)
 from celery.utils.objects import Bunch
 
 
 class test_DictAttribute:
 
     def test_get_set_keys_values_items(self):
         x = DictAttribute(Bunch())
@@ -444,7 +445,20 @@
     def test_pop_empty_no_default(self):
         b = BufferMap(10)
         with pytest.raises(b.Empty):
             b.take(1)
 
     def test_repr(self):
         assert repr(Messagebuffer(10, [1, 2, 3]))
+
+
+class test_ChainMap:
+
+    def test_observers_not_shared(self):
+        a = ChainMap()
+        b = ChainMap()
+        callback = Mock()
+        a.bind_to(callback)
+        b.update(x=1)
+        callback.assert_not_called()
+        a.update(x=1)
+        callback.assert_called_once_with(x=1)
```

### Comparing `celery-5.3.0rc2/t/unit/utils/test_debug.py` & `celery-5.3.1/t/unit/utils/test_debug.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/utils/test_deprecated.py` & `celery-5.3.1/t/unit/utils/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/utils/test_dispatcher.py` & `celery-5.3.1/t/unit/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/utils/test_functional.py` & `celery-5.3.1/t/unit/utils/test_functional.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/utils/test_graph.py` & `celery-5.3.1/t/unit/utils/test_graph.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/utils/test_imports.py` & `celery-5.3.1/t/unit/utils/test_imports.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/utils/test_local.py` & `celery-5.3.1/t/unit/utils/test_local.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/utils/test_pickle.py` & `celery-5.3.1/t/unit/utils/test_pickle.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/utils/test_platforms.py` & `celery-5.3.1/t/unit/utils/test_platforms.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/utils/test_saferepr.py` & `celery-5.3.1/t/unit/utils/test_saferepr.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/utils/test_serialization.py` & `celery-5.3.1/t/unit/utils/test_serialization.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/utils/test_sysinfo.py` & `celery-5.3.1/t/unit/utils/test_sysinfo.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/utils/test_term.py` & `celery-5.3.1/t/unit/utils/test_term.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/utils/test_text.py` & `celery-5.3.1/t/unit/utils/test_text.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/utils/test_threads.py` & `celery-5.3.1/t/unit/utils/test_threads.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/utils/test_time.py` & `celery-5.3.1/t/unit/utils/test_time.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/utils/test_timer2.py` & `celery-5.3.1/t/unit/utils/test_timer2.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/utils/test_utils.py` & `celery-5.3.1/t/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/worker/test_autoscale.py` & `celery-5.3.1/t/unit/worker/test_autoscale.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/worker/test_bootsteps.py` & `celery-5.3.1/t/unit/worker/test_bootsteps.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/worker/test_components.py` & `celery-5.3.1/t/unit/worker/test_components.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/worker/test_consumer.py` & `celery-5.3.1/t/unit/worker/test_consumer.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/worker/test_control.py` & `celery-5.3.1/t/unit/worker/test_control.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/worker/test_heartbeat.py` & `celery-5.3.1/t/unit/worker/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/worker/test_loops.py` & `celery-5.3.1/t/unit/worker/test_loops.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/worker/test_request.py` & `celery-5.3.1/t/unit/worker/test_request.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/worker/test_state.py` & `celery-5.3.1/t/unit/worker/test_state.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/worker/test_strategy.py` & `celery-5.3.1/t/unit/worker/test_strategy.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0rc2/t/unit/worker/test_worker.py` & `celery-5.3.1/t/unit/worker/test_worker.py`

 * *Files identical despite different names*

