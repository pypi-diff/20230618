# Comparing `tmp/django_simple_file_handler-0.3.2.tar.gz` & `tmp/django_simple_file_handler-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_simple_file_handler-0.3.2.tar", last modified: Thu Apr  7 18:47:26 2022, max compression
+gzip compressed data, was "django_simple_file_handler-0.3.3.tar", last modified: Sun Jun 18 20:27:55 2023, max compression
```

## Comparing `django_simple_file_handler-0.3.2.tar` & `django_simple_file_handler-0.3.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-04-07 18:47:26.450915 django_simple_file_handler-0.3.2/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1063 2021-12-23 20:39:53.000000 django_simple_file_handler-0.3.2/LICENSE
--rw-r--r--   0 jonathanrickard   (501) staff       (20)       92 2018-05-11 20:52:40.000000 django_simple_file_handler-0.3.2/MANIFEST.in
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    10110 2022-04-07 18:47:26.451006 django_simple_file_handler-0.3.2/PKG-INFO
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     9146 2021-07-02 21:02:24.000000 django_simple_file_handler-0.3.2/README.rst
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-04-07 18:47:26.445763 django_simple_file_handler-0.3.2/django_simple_file_handler/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2021-08-11 17:41:13.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/__init__.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     5692 2021-07-02 20:49:56.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/admin.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      290 2021-05-13 19:59:37.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/apps.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2429 2021-05-21 18:33:37.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/file_types.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-04-07 18:47:26.448677 django_simple_file_handler-0.3.2/django_simple_file_handler/migrations/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     7655 2021-07-02 21:13:43.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/migrations/0001_initial.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2052 2021-07-02 21:13:37.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/migrations/0002_auto_20180521_1545.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2303 2021-07-02 21:13:31.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/migrations/0003_auto_20180525_1035.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     2220 2021-07-02 21:13:26.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/migrations/0004_auto_20181005_1601.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      526 2021-07-02 21:13:20.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/migrations/0005_auto_20190124_1658.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     4138 2021-07-02 21:13:05.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/migrations/0006_auto_20190429_1949.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     5956 2021-07-02 21:12:53.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/migrations/0007_auto_20210514_1405.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      786 2021-07-02 21:12:53.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/migrations/0008_auto_20210702_1604.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-10-09 23:50:29.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/migrations/__init__.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    14987 2022-04-07 18:25:34.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/models.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      382 2019-08-16 20:53:36.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/runtests.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-04-07 18:47:26.448864 django_simple_file_handler-0.3.2/django_simple_file_handler/signals/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-09-25 21:02:03.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/signals/__init__.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      780 2020-01-28 20:51:03.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/signals/handlers.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-04-07 18:47:26.449108 django_simple_file_handler-0.3.2/django_simple_file_handler/templates/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    10244 2020-02-03 21:46:31.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/templates/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-04-07 18:47:26.449334 django_simple_file_handler-0.3.2/django_simple_file_handler/templates/django_simple_file_handler/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     8196 2018-09-28 19:27:34.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/templates/django_simple_file_handler/.DS_Store
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-04-07 18:47:26.449593 django_simple_file_handler-0.3.2/django_simple_file_handler/templates/django_simple_file_handler/tests/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      148 2018-03-12 20:50:14.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/templates/django_simple_file_handler/tests/pdf_test.html
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-04-07 18:47:26.450736 django_simple_file_handler-0.3.2/django_simple_file_handler/tests/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-05-11 17:49:29.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/tests/__init__.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     3157 2022-04-07 18:30:08.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/tests/functions.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1601 2020-01-28 18:33:20.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/tests/settings.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     6982 2022-04-07 18:30:08.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/tests/test_models.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1533 2019-08-15 18:16:34.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/tests/test_views.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      162 2020-01-09 17:14:00.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/tests/urls.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)      356 2020-01-09 16:44:15.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/urls.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1508 2022-04-07 18:25:34.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/validators.py
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1060 2019-02-20 20:01:51.000000 django_simple_file_handler-0.3.2/django_simple_file_handler/views.py
-drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2022-04-07 18:47:26.446765 django_simple_file_handler-0.3.2/django_simple_file_handler.egg-info/
--rw-r--r--   0 jonathanrickard   (501) staff       (20)    10110 2022-04-07 18:47:26.000000 django_simple_file_handler-0.3.2/django_simple_file_handler.egg-info/PKG-INFO
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1812 2022-04-07 18:47:26.000000 django_simple_file_handler-0.3.2/django_simple_file_handler.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        1 2022-04-07 18:47:26.000000 django_simple_file_handler-0.3.2/django_simple_file_handler.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanrickard   (501) staff       (20)       48 2022-04-07 18:47:26.000000 django_simple_file_handler-0.3.2/django_simple_file_handler.egg-info/requires.txt
--rw-r--r--   0 jonathanrickard   (501) staff       (20)       27 2022-04-07 18:47:26.000000 django_simple_file_handler-0.3.2/django_simple_file_handler.egg-info/top_level.txt
--rw-r--r--   0 jonathanrickard   (501) staff       (20)        1 2021-04-01 21:28:44.000000 django_simple_file_handler-0.3.2/django_simple_file_handler.egg-info/zip-safe
--rw-r--r--   0 jonathanrickard   (501) staff       (20)     1016 2022-04-07 18:47:26.451390 django_simple_file_handler-0.3.2/setup.cfg
--rw-r--r--   0 jonathanrickard   (501) staff       (20)       39 2021-04-01 21:24:13.000000 django_simple_file_handler-0.3.2/setup.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 20:27:55.749949 django_simple_file_handler-0.3.3/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1063 2022-12-24 16:51:34.000000 django_simple_file_handler-0.3.3/LICENSE
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)       92 2018-05-11 20:52:40.000000 django_simple_file_handler-0.3.3/MANIFEST.in
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    10189 2023-06-18 20:27:55.750091 django_simple_file_handler-0.3.3/PKG-INFO
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     9146 2021-07-02 21:02:24.000000 django_simple_file_handler-0.3.3/README.rst
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 20:27:55.744759 django_simple_file_handler-0.3.3/django_simple_file_handler/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2021-08-11 17:41:13.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/__init__.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     5692 2021-07-02 20:49:56.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/admin.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      290 2021-05-13 19:59:37.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/apps.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2429 2021-05-21 18:33:37.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/file_types.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 20:27:55.747754 django_simple_file_handler-0.3.3/django_simple_file_handler/migrations/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     7655 2021-07-02 21:13:43.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/migrations/0001_initial.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2052 2021-07-02 21:13:37.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/migrations/0002_auto_20180521_1545.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2303 2021-07-02 21:13:31.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/migrations/0003_auto_20180525_1035.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     2220 2021-07-02 21:13:26.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/migrations/0004_auto_20181005_1601.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      526 2021-07-02 21:13:20.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/migrations/0005_auto_20190124_1658.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     4138 2021-07-02 21:13:05.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/migrations/0006_auto_20190429_1949.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     5956 2021-07-02 21:12:53.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/migrations/0007_auto_20210514_1405.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      786 2021-07-02 21:12:53.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/migrations/0008_auto_20210702_1604.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-10-09 23:50:29.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/migrations/__init__.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    14987 2022-04-07 18:25:34.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/models.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      382 2019-08-16 20:53:36.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/runtests.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 20:27:55.747981 django_simple_file_handler-0.3.3/django_simple_file_handler/signals/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-09-25 21:02:03.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/signals/__init__.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      780 2020-01-28 20:51:03.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/signals/handlers.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 20:27:55.748135 django_simple_file_handler-0.3.3/django_simple_file_handler/templates/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    10244 2020-02-03 21:46:31.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/templates/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 20:27:55.748537 django_simple_file_handler-0.3.3/django_simple_file_handler/templates/django_simple_file_handler/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     8196 2018-09-28 19:27:34.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/templates/django_simple_file_handler/.DS_Store
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 20:27:55.748719 django_simple_file_handler-0.3.3/django_simple_file_handler/templates/django_simple_file_handler/tests/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      148 2018-03-12 20:50:14.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/templates/django_simple_file_handler/tests/pdf_test.html
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 20:27:55.749788 django_simple_file_handler-0.3.3/django_simple_file_handler/tests/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        0 2018-05-11 17:49:29.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/tests/__init__.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     3157 2022-04-07 18:30:08.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/tests/functions.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1601 2020-01-28 18:33:20.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/tests/settings.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     6982 2022-04-07 18:30:08.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/tests/test_models.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1533 2019-08-15 18:16:34.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/tests/test_views.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      162 2020-01-09 17:14:00.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/tests/urls.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)      356 2020-01-09 16:44:15.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/urls.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1508 2022-04-07 18:25:34.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/validators.py
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1060 2019-02-20 20:01:51.000000 django_simple_file_handler-0.3.3/django_simple_file_handler/views.py
+drwxr-xr-x   0 jonathanrickard   (501) staff       (20)        0 2023-06-18 20:27:55.745503 django_simple_file_handler-0.3.3/django_simple_file_handler.egg-info/
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)    10189 2023-06-18 20:27:55.000000 django_simple_file_handler-0.3.3/django_simple_file_handler.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1812 2023-06-18 20:27:55.000000 django_simple_file_handler-0.3.3/django_simple_file_handler.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        1 2023-06-18 20:27:55.000000 django_simple_file_handler-0.3.3/django_simple_file_handler.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)       48 2023-06-18 20:27:55.000000 django_simple_file_handler-0.3.3/django_simple_file_handler.egg-info/requires.txt
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)       27 2023-06-18 20:27:55.000000 django_simple_file_handler-0.3.3/django_simple_file_handler.egg-info/top_level.txt
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)        1 2021-04-01 21:28:44.000000 django_simple_file_handler-0.3.3/django_simple_file_handler.egg-info/zip-safe
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)     1073 2023-06-18 20:27:55.750620 django_simple_file_handler-0.3.3/setup.cfg
+-rw-r--r--   0 jonathanrickard   (501) staff       (20)       39 2021-04-01 21:24:13.000000 django_simple_file_handler-0.3.3/setup.py
```

### Comparing `django_simple_file_handler-0.3.2/LICENSE` & `django_simple_file_handler-0.3.3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright (c) 2015-22 Jonathan Rickard
+Copyright (c) 2015-23 Jonathan Rickard
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `django_simple_file_handler-0.3.2/PKG-INFO` & `django_simple_file_handler-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: django_simple_file_handler
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Django app for storing and processing documents and images
 Home-page: https://github.com/jonathanrickard/django-simple-file-handler
 Author: Jonathan Rickard
 Author-email: jonathan@jonathanrickard.com
 License: MIT License
 Keywords: django,files,images
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
 
 ==========================
 django-simple-file-handler
```

### Comparing `django_simple_file_handler-0.3.2/README.rst` & `django_simple_file_handler-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `django_simple_file_handler-0.3.2/django_simple_file_handler/admin.py` & `django_simple_file_handler-0.3.3/django_simple_file_handler/admin.py`

 * *Files identical despite different names*

### Comparing `django_simple_file_handler-0.3.2/django_simple_file_handler/file_types.py` & `django_simple_file_handler-0.3.3/django_simple_file_handler/file_types.py`

 * *Files identical despite different names*

### Comparing `django_simple_file_handler-0.3.2/django_simple_file_handler/migrations/0001_initial.py` & `django_simple_file_handler-0.3.3/django_simple_file_handler/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_simple_file_handler-0.3.2/django_simple_file_handler/migrations/0002_auto_20180521_1545.py` & `django_simple_file_handler-0.3.3/django_simple_file_handler/migrations/0002_auto_20180521_1545.py`

 * *Files identical despite different names*

### Comparing `django_simple_file_handler-0.3.2/django_simple_file_handler/migrations/0003_auto_20180525_1035.py` & `django_simple_file_handler-0.3.3/django_simple_file_handler/migrations/0003_auto_20180525_1035.py`

 * *Files identical despite different names*

### Comparing `django_simple_file_handler-0.3.2/django_simple_file_handler/migrations/0004_auto_20181005_1601.py` & `django_simple_file_handler-0.3.3/django_simple_file_handler/migrations/0004_auto_20181005_1601.py`

 * *Files identical despite different names*

### Comparing `django_simple_file_handler-0.3.2/django_simple_file_handler/migrations/0005_auto_20190124_1658.py` & `django_simple_file_handler-0.3.3/django_simple_file_handler/migrations/0005_auto_20190124_1658.py`

 * *Files identical despite different names*

### Comparing `django_simple_file_handler-0.3.2/django_simple_file_handler/migrations/0006_auto_20190429_1949.py` & `django_simple_file_handler-0.3.3/django_simple_file_handler/migrations/0006_auto_20190429_1949.py`

 * *Files identical despite different names*

### Comparing `django_simple_file_handler-0.3.2/django_simple_file_handler/migrations/0007_auto_20210514_1405.py` & `django_simple_file_handler-0.3.3/django_simple_file_handler/migrations/0007_auto_20210514_1405.py`

 * *Files identical despite different names*

### Comparing `django_simple_file_handler-0.3.2/django_simple_file_handler/migrations/0008_auto_20210702_1604.py` & `django_simple_file_handler-0.3.3/django_simple_file_handler/migrations/0008_auto_20210702_1604.py`

 * *Files identical despite different names*

### Comparing `django_simple_file_handler-0.3.2/django_simple_file_handler/models.py` & `django_simple_file_handler-0.3.3/django_simple_file_handler/models.py`

 * *Files identical despite different names*

### Comparing `django_simple_file_handler-0.3.2/django_simple_file_handler/signals/handlers.py` & `django_simple_file_handler-0.3.3/django_simple_file_handler/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `django_simple_file_handler-0.3.2/django_simple_file_handler/templates/.DS_Store` & `django_simple_file_handler-0.3.3/django_simple_file_handler/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_file_handler-0.3.2/django_simple_file_handler/templates/django_simple_file_handler/.DS_Store` & `django_simple_file_handler-0.3.3/django_simple_file_handler/templates/django_simple_file_handler/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_simple_file_handler-0.3.2/django_simple_file_handler/tests/functions.py` & `django_simple_file_handler-0.3.3/django_simple_file_handler/tests/functions.py`

 * *Files identical despite different names*

### Comparing `django_simple_file_handler-0.3.2/django_simple_file_handler/tests/settings.py` & `django_simple_file_handler-0.3.3/django_simple_file_handler/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_simple_file_handler-0.3.2/django_simple_file_handler/tests/test_models.py` & `django_simple_file_handler-0.3.3/django_simple_file_handler/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_simple_file_handler-0.3.2/django_simple_file_handler/tests/test_views.py` & `django_simple_file_handler-0.3.3/django_simple_file_handler/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_simple_file_handler-0.3.2/django_simple_file_handler/validators.py` & `django_simple_file_handler-0.3.3/django_simple_file_handler/validators.py`

 * *Files identical despite different names*

### Comparing `django_simple_file_handler-0.3.2/django_simple_file_handler/views.py` & `django_simple_file_handler-0.3.3/django_simple_file_handler/views.py`

 * *Files identical despite different names*

### Comparing `django_simple_file_handler-0.3.2/django_simple_file_handler.egg-info/PKG-INFO` & `django_simple_file_handler-0.3.3/django_simple_file_handler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: django-simple-file-handler
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Django app for storing and processing documents and images
 Home-page: https://github.com/jonathanrickard/django-simple-file-handler
 Author: Jonathan Rickard
 Author-email: jonathan@jonathanrickard.com
 License: MIT License
 Keywords: django,files,images
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
 
 ==========================
 django-simple-file-handler
```

### Comparing `django_simple_file_handler-0.3.2/django_simple_file_handler.egg-info/SOURCES.txt` & `django_simple_file_handler-0.3.3/django_simple_file_handler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

