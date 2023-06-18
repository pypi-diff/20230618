# Comparing `tmp/Bigsansar-1.7.1.tar.gz` & `tmp/Bigsansar-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bigsansar-1.7.1.tar", last modified: Fri Jun  9 12:51:12 2023, max compression
+gzip compressed data, was "Bigsansar-1.7.2.tar", last modified: Sun Jun 18 02:46:32 2023, max compression
```

## Comparing `Bigsansar-1.7.1.tar` & `Bigsansar-1.7.2.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.790699 Bigsansar-1.7.1/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.710699 Bigsansar-1.7.1/Bigsansar.egg-info/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4603 2023-06-09 12:51:12.000000 Bigsansar-1.7.1/Bigsansar.egg-info/PKG-INFO
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4913 2023-06-09 12:51:12.000000 Bigsansar-1.7.1/Bigsansar.egg-info/SOURCES.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2023-06-09 12:51:12.000000 Bigsansar-1.7.1/Bigsansar.egg-info/dependency_links.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       51 2023-06-09 12:51:12.000000 Bigsansar-1.7.1/Bigsansar.egg-info/entry_points.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       98 2023-06-09 12:51:12.000000 Bigsansar-1.7.1/Bigsansar.egg-info/requires.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2023-06-09 12:51:12.000000 Bigsansar-1.7.1/Bigsansar.egg-info/top_level.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1091 2023-04-29 06:46:12.000000 Bigsansar-1.7.1/LICENSE
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4603 2023-06-09 12:51:12.790699 Bigsansar-1.7.1/PKG-INFO
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4033 2023-06-09 12:50:57.000000 Bigsansar-1.7.1/README.md
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.720699 Bigsansar-1.7.1/bigsansar/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.720699 Bigsansar-1.7.1/bigsansar/contrib/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.720699 Bigsansar-1.7.1/bigsansar/contrib/account/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/account/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      510 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/account/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      284 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/account/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1176 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/account/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.720699 Bigsansar-1.7.1/bigsansar/contrib/account/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      999 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/account/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/account/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      556 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/account/models.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      351 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/account/signals.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.720699 Bigsansar-1.7.1/bigsansar/contrib/account/templates/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/account/templates/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/account/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/account/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/account/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.730699 Bigsansar-1.7.1/bigsansar/contrib/advance/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.7.1/bigsansar/contrib/advance/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      291 2023-05-13 03:12:35.000000 Bigsansar-1.7.1/bigsansar/contrib/advance/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      202 2023-05-08 12:23:18.000000 Bigsansar-1.7.1/bigsansar/contrib/advance/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.730699 Bigsansar-1.7.1/bigsansar/contrib/advance/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1000 2023-05-08 12:29:40.000000 Bigsansar-1.7.1/bigsansar/contrib/advance/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      367 2023-05-13 02:56:41.000000 Bigsansar-1.7.1/bigsansar/contrib/advance/migrations/0002_alter_css_options.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1050 2023-05-13 03:08:43.000000 Bigsansar-1.7.1/bigsansar/contrib/advance/migrations/0003_javascript.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      386 2023-05-13 03:14:07.000000 Bigsansar-1.7.1/bigsansar/contrib/advance/migrations/0004_alter_javascript_options.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.7.1/bigsansar/contrib/advance/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1059 2023-05-13 04:58:52.000000 Bigsansar-1.7.1/bigsansar/contrib/advance/models.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-05-08 12:18:38.000000 Bigsansar-1.7.1/bigsansar/contrib/advance/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-05-08 12:18:38.000000 Bigsansar-1.7.1/bigsansar/contrib/advance/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.730699 Bigsansar-1.7.1/bigsansar/contrib/blogs/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/blogs/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2310 2023-06-09 12:48:58.000000 Bigsansar-1.7.1/bigsansar/contrib/blogs/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/blogs/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      261 2023-06-05 06:44:01.000000 Bigsansar-1.7.1/bigsansar/contrib/blogs/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.730699 Bigsansar-1.7.1/bigsansar/contrib/blogs/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2261 2023-05-29 10:57:40.000000 Bigsansar-1.7.1/bigsansar/contrib/blogs/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      367 2023-06-02 13:13:53.000000 Bigsansar-1.7.1/bigsansar/contrib/blogs/migrations/0002_post_visitor.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 10:57:14.000000 Bigsansar-1.7.1/bigsansar/contrib/blogs/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2152 2023-06-02 13:13:06.000000 Bigsansar-1.7.1/bigsansar/contrib/blogs/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.730699 Bigsansar-1.7.1/bigsansar/contrib/blogs/templatetags/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-20 12:33:35.000000 Bigsansar-1.7.1/bigsansar/contrib/blogs/templatetags/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1525 2023-06-05 06:21:13.000000 Bigsansar-1.7.1/bigsansar/contrib/blogs/templatetags/blogs.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/blogs/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/blogs/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.730699 Bigsansar-1.7.1/bigsansar/contrib/sites/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/sites/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2462 2023-06-09 12:43:48.000000 Bigsansar-1.7.1/bigsansar/contrib/sites/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      203 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/sites/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3579 2023-06-03 02:16:10.000000 Bigsansar-1.7.1/bigsansar/contrib/sites/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.730699 Bigsansar-1.7.1/bigsansar/contrib/sites/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1847 2023-05-02 12:46:38.000000 Bigsansar-1.7.1/bigsansar/contrib/sites/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:46:31.000000 Bigsansar-1.7.1/bigsansar/contrib/sites/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1899 2023-05-17 10:15:27.000000 Bigsansar-1.7.1/bigsansar/contrib/sites/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.730699 Bigsansar-1.7.1/bigsansar/contrib/sites/templatetags/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/sites/templatetags/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/sites/templatetags/pages.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/sites/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/contrib/sites/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.730699 Bigsansar-1.7.1/bigsansar/core/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      524 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/core/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      414 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/core/host.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    10679 2023-05-27 06:38:55.000000 Bigsansar-1.7.1/bigsansar/core/init.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       27 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/main.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.740699 Bigsansar-1.7.1/bigsansar/management/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/management/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.740699 Bigsansar-1.7.1/bigsansar/management/commands/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/management/commands/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1122 2023-04-27 12:44:33.000000 Bigsansar-1.7.1/bigsansar/management/commands/createuser.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.740699 Bigsansar-1.7.1/bigsansar/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.740699 Bigsansar-1.7.1/bigsansar/static/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/static/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.710699 Bigsansar-1.7.1/bigsansar/static/ckeditor/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.710699 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.710699 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.740699 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.750699 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1258 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1165 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.780699 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1337 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1654 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1209 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1078 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1514 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1049 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1084 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1103 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1186 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      960 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1051 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1250 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1166 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1106 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1195 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1229 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1059 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1047 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1064 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1120 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1151 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1178 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1564 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1173 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1206 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1538 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1067 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      916 2021-03-31 11:22:53.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    13371 2021-03-31 14:36:18.000000 Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9230 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/static/logo.png
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      525 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/static/style.css
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-09 12:51:12.790699 Bigsansar-1.7.1/bigsansar/templates/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      977 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/templates/404.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/templates/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      168 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/templates/acc_active_email.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1521 2023-05-05 10:08:59.000000 Bigsansar-1.7.1/bigsansar/templates/base.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1931 2023-06-05 06:55:58.000000 Bigsansar-1.7.1/bigsansar/templates/blog_preview.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2252 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/templates/default.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2250 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/templates/defaultpage.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      758 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/templates/parking.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-06-06 04:42:17.000000 Bigsansar-1.7.1/bigsansar/templates/sitemap.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.7.1/bigsansar/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1155 2023-05-20 14:08:47.000000 Bigsansar-1.7.1/bigsansar/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4479 2023-06-05 06:54:06.000000 Bigsansar-1.7.1/bigsansar/views.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2023-06-09 12:51:12.790699 Bigsansar-1.7.1/setup.cfg
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1712 2023-06-09 12:20:56.000000 Bigsansar-1.7.1/setup.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.648793 Bigsansar-1.7.2/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.568792 Bigsansar-1.7.2/Bigsansar.egg-info/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4620 2023-06-18 02:46:32.000000 Bigsansar-1.7.2/Bigsansar.egg-info/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4913 2023-06-18 02:46:32.000000 Bigsansar-1.7.2/Bigsansar.egg-info/SOURCES.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2023-06-18 02:46:32.000000 Bigsansar-1.7.2/Bigsansar.egg-info/dependency_links.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       51 2023-06-18 02:46:32.000000 Bigsansar-1.7.2/Bigsansar.egg-info/entry_points.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       98 2023-06-18 02:46:32.000000 Bigsansar-1.7.2/Bigsansar.egg-info/requires.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2023-06-18 02:46:32.000000 Bigsansar-1.7.2/Bigsansar.egg-info/top_level.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1091 2023-04-29 06:46:12.000000 Bigsansar-1.7.2/LICENSE
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4620 2023-06-18 02:46:32.648793 Bigsansar-1.7.2/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4050 2023-06-18 02:45:42.000000 Bigsansar-1.7.2/README.md
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.568792 Bigsansar-1.7.2/bigsansar/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.568792 Bigsansar-1.7.2/bigsansar/contrib/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.578792 Bigsansar-1.7.2/bigsansar/contrib/account/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/account/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      510 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/account/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      284 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/account/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1176 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/account/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.588792 Bigsansar-1.7.2/bigsansar/contrib/account/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      999 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/account/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/account/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      556 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/account/models.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      351 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/account/signals.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.588792 Bigsansar-1.7.2/bigsansar/contrib/account/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/account/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/account/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/account/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/account/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.588792 Bigsansar-1.7.2/bigsansar/contrib/advance/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.7.2/bigsansar/contrib/advance/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      291 2023-05-13 03:12:35.000000 Bigsansar-1.7.2/bigsansar/contrib/advance/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      202 2023-05-08 12:23:18.000000 Bigsansar-1.7.2/bigsansar/contrib/advance/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.588792 Bigsansar-1.7.2/bigsansar/contrib/advance/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1000 2023-05-08 12:29:40.000000 Bigsansar-1.7.2/bigsansar/contrib/advance/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      367 2023-05-13 02:56:41.000000 Bigsansar-1.7.2/bigsansar/contrib/advance/migrations/0002_alter_css_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1050 2023-05-13 03:08:43.000000 Bigsansar-1.7.2/bigsansar/contrib/advance/migrations/0003_javascript.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      386 2023-05-13 03:14:07.000000 Bigsansar-1.7.2/bigsansar/contrib/advance/migrations/0004_alter_javascript_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.7.2/bigsansar/contrib/advance/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1059 2023-05-13 04:58:52.000000 Bigsansar-1.7.2/bigsansar/contrib/advance/models.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-05-08 12:18:38.000000 Bigsansar-1.7.2/bigsansar/contrib/advance/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-05-08 12:18:38.000000 Bigsansar-1.7.2/bigsansar/contrib/advance/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.588792 Bigsansar-1.7.2/bigsansar/contrib/blogs/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/blogs/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2302 2023-06-16 11:18:51.000000 Bigsansar-1.7.2/bigsansar/contrib/blogs/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/blogs/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      261 2023-06-05 06:44:01.000000 Bigsansar-1.7.2/bigsansar/contrib/blogs/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.588792 Bigsansar-1.7.2/bigsansar/contrib/blogs/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2261 2023-05-29 10:57:40.000000 Bigsansar-1.7.2/bigsansar/contrib/blogs/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      367 2023-06-02 13:13:53.000000 Bigsansar-1.7.2/bigsansar/contrib/blogs/migrations/0002_post_visitor.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 10:57:14.000000 Bigsansar-1.7.2/bigsansar/contrib/blogs/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2152 2023-06-02 13:13:06.000000 Bigsansar-1.7.2/bigsansar/contrib/blogs/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.588792 Bigsansar-1.7.2/bigsansar/contrib/blogs/templatetags/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-20 12:33:35.000000 Bigsansar-1.7.2/bigsansar/contrib/blogs/templatetags/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1525 2023-06-05 06:21:13.000000 Bigsansar-1.7.2/bigsansar/contrib/blogs/templatetags/blogs.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/blogs/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/blogs/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.588792 Bigsansar-1.7.2/bigsansar/contrib/sites/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/sites/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2462 2023-06-09 12:43:48.000000 Bigsansar-1.7.2/bigsansar/contrib/sites/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      203 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/sites/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3579 2023-06-03 02:16:10.000000 Bigsansar-1.7.2/bigsansar/contrib/sites/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.588792 Bigsansar-1.7.2/bigsansar/contrib/sites/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1847 2023-05-02 12:46:38.000000 Bigsansar-1.7.2/bigsansar/contrib/sites/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:46:31.000000 Bigsansar-1.7.2/bigsansar/contrib/sites/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1899 2023-05-17 10:15:27.000000 Bigsansar-1.7.2/bigsansar/contrib/sites/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.598792 Bigsansar-1.7.2/bigsansar/contrib/sites/templatetags/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/sites/templatetags/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/sites/templatetags/pages.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/sites/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/contrib/sites/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.598792 Bigsansar-1.7.2/bigsansar/core/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      524 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/core/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      414 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/core/host.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    10679 2023-05-27 06:38:55.000000 Bigsansar-1.7.2/bigsansar/core/init.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       27 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/main.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.598792 Bigsansar-1.7.2/bigsansar/management/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/management/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.598792 Bigsansar-1.7.2/bigsansar/management/commands/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/management/commands/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1122 2023-04-27 12:44:33.000000 Bigsansar-1.7.2/bigsansar/management/commands/createuser.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.598792 Bigsansar-1.7.2/bigsansar/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.598792 Bigsansar-1.7.2/bigsansar/static/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/static/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.558792 Bigsansar-1.7.2/bigsansar/static/ckeditor/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.558792 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.568792 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.598792 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.598792 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1258 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1165 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.638792 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1337 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1654 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1209 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1078 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1514 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1049 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1084 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1103 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1186 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      960 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1051 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1250 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1166 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1106 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1195 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1229 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1059 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1047 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1064 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1120 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1151 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1178 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1564 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1173 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1206 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1538 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1067 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      916 2021-03-31 11:22:53.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    13371 2021-03-31 14:36:18.000000 Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9230 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/static/logo.png
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      525 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/static/style.css
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-18 02:46:32.648793 Bigsansar-1.7.2/bigsansar/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      977 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/templates/404.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      168 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/templates/acc_active_email.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1521 2023-05-05 10:08:59.000000 Bigsansar-1.7.2/bigsansar/templates/base.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1931 2023-06-05 06:55:58.000000 Bigsansar-1.7.2/bigsansar/templates/blog_preview.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2252 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/templates/default.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2250 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/templates/defaultpage.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      758 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/templates/parking.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-06-06 04:42:17.000000 Bigsansar-1.7.2/bigsansar/templates/sitemap.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.7.2/bigsansar/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1155 2023-05-20 14:08:47.000000 Bigsansar-1.7.2/bigsansar/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4719 2023-06-18 02:41:07.000000 Bigsansar-1.7.2/bigsansar/views.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2023-06-18 02:46:32.648793 Bigsansar-1.7.2/setup.cfg
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1712 2023-06-18 02:45:48.000000 Bigsansar-1.7.2/setup.py
```

### Comparing `Bigsansar-1.7.1/Bigsansar.egg-info/PKG-INFO` & `Bigsansar-1.7.2/Bigsansar.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.7.1
+Version: 1.7.2
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
@@ -14,19 +14,19 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## New update
+* now sitemap system can add or edit manually 
 * fixed control system for superuser and normal user in to custom domain and blog post modols.
 * fixed visitor system in to blog post.
 * added thumbnails model field in blog system
 * added sitmap system 
-* added font awesome packages
 
  
 # How to get Bigsansar
 
 Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3.
 Bigsansar is Fully based on django.
 You can use
```

#### html2text {}

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1 Name: Bigsansar Version: 1.7.1 Summary: Build one in
+Metadata-Version: 2.1 Name: Bigsansar Version: 1.7.2 Summary: Build one in
 minutes with bigsansar - a visual site building tool! Home-page: https://
 bigsansar.com Author: Bikash Pokhrel Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN Project-URL: Bug Tracker, https://github.com/pokhrelb9/
 bigsansar/issues Project-URL: Documentations, https://docs.bigsansar.com/
 Keywords: python,django host,bigsansar,django,django sites framework,django
 flatpages Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
-markdown License-File: LICENSE ## New update * fixed control system for
-superuser and normal user in to custom domain and blog post modols. * fixed
-visitor system in to blog post. * added thumbnails model field in blog system *
-added sitmap system * added font awesome packages # How to get Bigsansar
-Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/
-wiki/MIT_License) license. We recommend using the latest version of Python 3.
-Bigsansar is Fully based on django. You can use [bigsansar](https://
-bigsansar.com) for install packaged. view our tutorials in [youtube](https://
-youtube.com/bigsansar) for playlist: [bigsansar for django](https://
-www.youtube.com/playlist?list=PLqdXqRSrD-LC6i7YQAaqB57FaCfWEZkth) # Get the
-latest development version The latest and greatest Bigsasnar version is the one
-thatâs in our Git repository (our revision-control system). This is only for
-experienced users who want to try incoming changes and help identify bugs
-before an official release. Get it using this shell command, which requires
-[Git](https://git-scm.com/): `git clone https://github.com/pokhrelb9/
+markdown License-File: LICENSE ## New update * now sitemap system can add or
+edit manually * fixed control system for superuser and normal user in to custom
+domain and blog post modols. * fixed visitor system in to blog post. * added
+thumbnails model field in blog system * added sitmap system # How to get
+Bigsansar Bigsansar is available open-source under the [MIT](https://
+en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest
+version of Python 3. Bigsansar is Fully based on django. You can use
+[bigsansar](https://bigsansar.com) for install packaged. view our tutorials in
+[youtube](https://youtube.com/bigsansar) for playlist: [bigsansar for django]
+(https://www.youtube.com/playlist?list=PLqdXqRSrD-LC6i7YQAaqB57FaCfWEZkth) #
+Get the latest development version The latest and greatest Bigsasnar version is
+the one thatâs in our Git repository (our revision-control system). This is
+only for experienced users who want to try incoming changes and help identify
+bugs before an official release. Get it using this shell command, which
+requires [Git](https://git-scm.com/): `git clone https://github.com/pokhrelb9/
 bigsansar.git` You can also download a [gzipped tarball](https://pypi.org/
 project/Bigsansar/#files) of the development version. This archive is updated
 every time we commit code. # After you install bigsansar Type `bigsansar init`
 command for **automatically** setup server . # How to access admin pannel in
 local env Go to [localhost:8000](http://localhost:8000) # How to change admin
 URL in server side with domain go to **VirtualHost.py** file and change
 **localhost:8000** with your subdomain ## Some usefull commands: `python3
```

### Comparing `Bigsansar-1.7.1/Bigsansar.egg-info/SOURCES.txt` & `Bigsansar-1.7.2/Bigsansar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/LICENSE` & `Bigsansar-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/PKG-INFO` & `Bigsansar-1.7.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.7.1
+Version: 1.7.2
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
@@ -14,19 +14,19 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## New update
+* now sitemap system can add or edit manually 
 * fixed control system for superuser and normal user in to custom domain and blog post modols.
 * fixed visitor system in to blog post.
 * added thumbnails model field in blog system
 * added sitmap system 
-* added font awesome packages
 
  
 # How to get Bigsansar
 
 Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3.
 Bigsansar is Fully based on django.
 You can use
```

#### html2text {}

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1 Name: Bigsansar Version: 1.7.1 Summary: Build one in
+Metadata-Version: 2.1 Name: Bigsansar Version: 1.7.2 Summary: Build one in
 minutes with bigsansar - a visual site building tool! Home-page: https://
 bigsansar.com Author: Bikash Pokhrel Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN Project-URL: Bug Tracker, https://github.com/pokhrelb9/
 bigsansar/issues Project-URL: Documentations, https://docs.bigsansar.com/
 Keywords: python,django host,bigsansar,django,django sites framework,django
 flatpages Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
-markdown License-File: LICENSE ## New update * fixed control system for
-superuser and normal user in to custom domain and blog post modols. * fixed
-visitor system in to blog post. * added thumbnails model field in blog system *
-added sitmap system * added font awesome packages # How to get Bigsansar
-Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/
-wiki/MIT_License) license. We recommend using the latest version of Python 3.
-Bigsansar is Fully based on django. You can use [bigsansar](https://
-bigsansar.com) for install packaged. view our tutorials in [youtube](https://
-youtube.com/bigsansar) for playlist: [bigsansar for django](https://
-www.youtube.com/playlist?list=PLqdXqRSrD-LC6i7YQAaqB57FaCfWEZkth) # Get the
-latest development version The latest and greatest Bigsasnar version is the one
-thatâs in our Git repository (our revision-control system). This is only for
-experienced users who want to try incoming changes and help identify bugs
-before an official release. Get it using this shell command, which requires
-[Git](https://git-scm.com/): `git clone https://github.com/pokhrelb9/
+markdown License-File: LICENSE ## New update * now sitemap system can add or
+edit manually * fixed control system for superuser and normal user in to custom
+domain and blog post modols. * fixed visitor system in to blog post. * added
+thumbnails model field in blog system * added sitmap system # How to get
+Bigsansar Bigsansar is available open-source under the [MIT](https://
+en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest
+version of Python 3. Bigsansar is Fully based on django. You can use
+[bigsansar](https://bigsansar.com) for install packaged. view our tutorials in
+[youtube](https://youtube.com/bigsansar) for playlist: [bigsansar for django]
+(https://www.youtube.com/playlist?list=PLqdXqRSrD-LC6i7YQAaqB57FaCfWEZkth) #
+Get the latest development version The latest and greatest Bigsasnar version is
+the one thatâs in our Git repository (our revision-control system). This is
+only for experienced users who want to try incoming changes and help identify
+bugs before an official release. Get it using this shell command, which
+requires [Git](https://git-scm.com/): `git clone https://github.com/pokhrelb9/
 bigsansar.git` You can also download a [gzipped tarball](https://pypi.org/
 project/Bigsansar/#files) of the development version. This archive is updated
 every time we commit code. # After you install bigsansar Type `bigsansar init`
 command for **automatically** setup server . # How to access admin pannel in
 local env Go to [localhost:8000](http://localhost:8000) # How to change admin
 URL in server side with domain go to **VirtualHost.py** file and change
 **localhost:8000** with your subdomain ## Some usefull commands: `python3
```

### Comparing `Bigsansar-1.7.1/README.md` & `Bigsansar-1.7.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ## New update
+* now sitemap system can add or edit manually 
 * fixed control system for superuser and normal user in to custom domain and blog post modols.
 * fixed visitor system in to blog post.
 * added thumbnails model field in blog system
 * added sitmap system 
-* added font awesome packages
 
  
 # How to get Bigsansar
 
 Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3.
 Bigsansar is Fully based on django.
 You can use
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-## New update * fixed control system for superuser and normal user in to custom
-domain and blog post modols. * fixed visitor system in to blog post. * added
-thumbnails model field in blog system * added sitmap system * added font
-awesome packages # How to get Bigsansar Bigsansar is available open-source
-under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We
-recommend using the latest version of Python 3. Bigsansar is Fully based on
+## New update * now sitemap system can add or edit manually * fixed control
+system for superuser and normal user in to custom domain and blog post modols.
+* fixed visitor system in to blog post. * added thumbnails model field in blog
+system * added sitmap system # How to get Bigsansar Bigsansar is available
+open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license.
+We recommend using the latest version of Python 3. Bigsansar is Fully based on
 django. You can use [bigsansar](https://bigsansar.com) for install packaged.
 view our tutorials in [youtube](https://youtube.com/bigsansar) for playlist:
 [bigsansar for django](https://www.youtube.com/playlist?list=PLqdXqRSrD-
 LC6i7YQAaqB57FaCfWEZkth) # Get the latest development version The latest and
 greatest Bigsasnar version is the one thatâs in our Git repository (our
 revision-control system). This is only for experienced users who want to try
 incoming changes and help identify bugs before an official release. Get it
```

### Comparing `Bigsansar-1.7.1/bigsansar/contrib/account/forms.py` & `Bigsansar-1.7.2/bigsansar/contrib/account/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/contrib/account/migrations/0001_initial.py` & `Bigsansar-1.7.2/bigsansar/contrib/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/contrib/account/models.py` & `Bigsansar-1.7.2/bigsansar/contrib/account/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/contrib/advance/migrations/0001_initial.py` & `Bigsansar-1.7.2/bigsansar/contrib/advance/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/contrib/advance/migrations/0003_javascript.py` & `Bigsansar-1.7.2/bigsansar/contrib/advance/migrations/0003_javascript.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/contrib/advance/models.py` & `Bigsansar-1.7.2/bigsansar/contrib/advance/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/contrib/blogs/admin.py` & `Bigsansar-1.7.2/bigsansar/contrib/blogs/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         # This is where you process parameters selected by use via filter options:
         if self.value():
             return queryset.filter(domain=self.value(), user=request.user)
 
 
 class blogadmin(admin.ModelAdmin):
     form = customblogform
-    list_display = ['title', 'user', 'publish_date', 'visitor']
+    list_display = ['title', 'publish_date', 'visitor']
     prepopulated_fields = {"slug": ("title",)}
     search_fields = ['title']
     list_filter = (domain_filter,)
 
     def get_queryset(self, request):
         qs = super().get_queryset(request)
         if request.user.is_superuser:
```

### Comparing `Bigsansar-1.7.1/bigsansar/contrib/blogs/migrations/0001_initial.py` & `Bigsansar-1.7.2/bigsansar/contrib/blogs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/contrib/blogs/models.py` & `Bigsansar-1.7.2/bigsansar/contrib/blogs/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/contrib/blogs/templatetags/blogs.py` & `Bigsansar-1.7.2/bigsansar/contrib/blogs/templatetags/blogs.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/contrib/sites/admin.py` & `Bigsansar-1.7.2/bigsansar/contrib/sites/admin.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/contrib/sites/forms.py` & `Bigsansar-1.7.2/bigsansar/contrib/sites/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/contrib/sites/migrations/0001_initial.py` & `Bigsansar-1.7.2/bigsansar/contrib/sites/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/contrib/sites/models.py` & `Bigsansar-1.7.2/bigsansar/contrib/sites/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/core/__init__.py` & `Bigsansar-1.7.2/bigsansar/core/__init__.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/core/init.py` & `Bigsansar-1.7.2/bigsansar/core/init.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/management/commands/createuser.py` & `Bigsansar-1.7.2/bigsansar/management/commands/createuser.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js` & `Bigsansar-1.7.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/logo.png` & `Bigsansar-1.7.2/bigsansar/static/logo.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/static/style.css` & `Bigsansar-1.7.2/bigsansar/static/style.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/templates/404.html` & `Bigsansar-1.7.2/bigsansar/templates/404.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/templates/base.html` & `Bigsansar-1.7.2/bigsansar/templates/base.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/templates/blog_preview.html` & `Bigsansar-1.7.2/bigsansar/templates/blog_preview.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/templates/default.html` & `Bigsansar-1.7.2/bigsansar/templates/default.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/templates/defaultpage.html` & `Bigsansar-1.7.2/bigsansar/templates/defaultpage.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/templates/parking.html` & `Bigsansar-1.7.2/bigsansar/templates/parking.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/urls.py` & `Bigsansar-1.7.2/bigsansar/urls.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.7.1/bigsansar/views.py` & `Bigsansar-1.7.2/bigsansar/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,23 +107,29 @@
 
         getjavahttp = HttpResponse(get_javascript.javascript)
         getjavahttp['Content-Type'] = 'text/javascript'
         return getjavahttp
     
 
 def sitemap(request):
+    default_page = 'sitemap.html'
+
     try:
         current_site = get_current_site(request)
-        domains.objects.get(domain=current_site)
+        db = domains.objects.get(domain=current_site)
+        page = pages.objects.get(domain=db, slug='sitemap')
+
     except:
         return render(request, '404.html')
     
     else:
-        template = loader.get_template('sitemap.html')
-        getsitemaphttp = HttpResponse(template.render({}, request))
+        asp = 'templates/' + str(db.domain) + '/' + page.slug + '.html'
+        full_url = os.path.join(BASE_DIR, asp)
+        template = loader.select_template((full_url, default_page))
+        getsitemaphttp =  HttpResponse(template.render({}, request))
         getsitemaphttp['Content-Type'] = 'application/xml'
         return getsitemaphttp
 
 
 def blog_preview(request,id):
     try:
         current_site = get_current_site(request)
```

### Comparing `Bigsansar-1.7.1/setup.py` & `Bigsansar-1.7.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Bigsansar",
-    version="1.7.1",
+    version="1.7.2",
     author="Bikash Pokhrel",
     author_email="bigsansaroffice@gmail.com",
     description="Build one in minutes with bigsansar - a visual site building tool!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bigsansar.com",
     project_urls={
```

