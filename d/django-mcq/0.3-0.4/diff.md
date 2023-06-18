# Comparing `tmp/django-mcq-0.3.tar.gz` & `tmp/django-mcq-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mcq-0.3.tar", last modified: Sun May 14 04:15:48 2023, max compression
+gzip compressed data, was "django-mcq-0.4.tar", last modified: Sun Jun 18 06:11:03 2023, max compression
```

## Comparing `django-mcq-0.3.tar` & `django-mcq-0.4.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-14 04:15:48.031310 django-mcq-0.3/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1063 2023-05-01 02:01:55.000000 django-mcq-0.3/LICENSE
--rw-rw-r--   0 suhail    (1000) suhail    (1000)       61 2023-05-01 02:23:43.000000 django-mcq-0.3/MANIFEST.in
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1795 2023-05-14 04:15:48.031310 django-mcq-0.3/PKG-INFO
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1044 2023-05-14 04:13:58.000000 django-mcq-0.3/README.md
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-14 04:15:48.027303 django-mcq-0.3/django_mcq.egg-info/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1795 2023-05-14 04:15:48.000000 django-mcq-0.3/django_mcq.egg-info/PKG-INFO
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1110 2023-05-14 04:15:48.000000 django-mcq-0.3/django_mcq.egg-info/SOURCES.txt
--rw-rw-r--   0 suhail    (1000) suhail    (1000)        1 2023-05-14 04:15:48.000000 django-mcq-0.3/django_mcq.egg-info/dependency_links.txt
--rw-rw-r--   0 suhail    (1000) suhail    (1000)        1 2023-05-01 02:49:00.000000 django-mcq-0.3/django_mcq.egg-info/not-zip-safe
--rw-rw-r--   0 suhail    (1000) suhail    (1000)       14 2023-05-14 04:15:48.000000 django-mcq-0.3/django_mcq.egg-info/requires.txt
--rw-rw-r--   0 suhail    (1000) suhail    (1000)        5 2023-05-14 04:15:48.000000 django-mcq-0.3/django_mcq.egg-info/top_level.txt
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      104 2023-05-01 02:01:55.000000 django-mcq-0.3/pyproject.toml
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-14 04:15:48.027303 django-mcq-0.3/quiz/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/__init__.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)       63 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/admin.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      140 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/apps.py
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-14 04:15:48.027303 django-mcq-0.3/quiz/fixtures/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)    16766 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/fixtures/sample_quizzes.json
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      879 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/forms.py
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-14 04:15:48.027303 django-mcq-0.3/quiz/migrations/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     6373 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/migrations/0001_initial.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/migrations/__init__.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     2655 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/models.py
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-14 04:15:48.023296 django-mcq-0.3/quiz/static/
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-14 04:15:48.027303 django-mcq-0.3/quiz/static/datatables/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     5222 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/static/datatables/dataTables.bootstrap4.min.css
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     2085 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/static/datatables/dataTables.bootstrap4.min.js
--rw-rw-r--   0 suhail    (1000) suhail    (1000)    82411 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/static/datatables/jquery.dataTables.min.js
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-14 04:15:48.027303 django-mcq-0.3/quiz/static/quiz/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      533 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/static/quiz/app.css
--rw-rw-r--   0 suhail    (1000) suhail    (1000)   141997 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/static/quiz/bootstrap.min.css
--rw-rw-r--   0 suhail    (1000) suhail    (1000)    86927 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/static/quiz/jquery-3.3.1.min.js
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-14 04:15:48.023296 django-mcq-0.3/quiz/templates/
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-14 04:15:48.031310 django-mcq-0.3/quiz/templates/quiz/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      670 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/templates/quiz/_header.html
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      801 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/templates/quiz/base.html
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      384 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/templates/quiz/interests_form.html
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     3478 2023-05-14 04:12:39.000000 django-mcq-0.3/quiz/templates/quiz/quiz_list.html
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1683 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/templates/quiz/quiz_result.html
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1251 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/templates/quiz/student_detail.html
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     2396 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/templates/quiz/student_list.html
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      685 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/templates/quiz/take_quiz_form.html
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      847 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/templates/quiz/taken_quiz_list.html
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-14 04:15:48.031310 django-mcq-0.3/quiz/templatetags/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/templatetags/__init__.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      995 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/templatetags/quiz_extras.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)       60 2023-05-01 02:01:55.000000 django-mcq-0.3/quiz/tests.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      724 2023-05-14 04:12:39.000000 django-mcq-0.3/quiz/urls.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     8036 2023-05-14 04:12:39.000000 django-mcq-0.3/quiz/views.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)       38 2023-05-14 04:15:48.031310 django-mcq-0.3/setup.cfg
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1078 2023-05-14 04:13:09.000000 django-mcq-0.3/setup.py
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-06-18 06:11:03.303757 django-mcq-0.4/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1063 2023-05-01 02:01:55.000000 django-mcq-0.4/LICENSE
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)       61 2023-05-01 02:23:43.000000 django-mcq-0.4/MANIFEST.in
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1795 2023-06-18 06:11:03.303757 django-mcq-0.4/PKG-INFO
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1044 2023-05-14 04:13:58.000000 django-mcq-0.4/README.md
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-06-18 06:11:03.283758 django-mcq-0.4/django_mcq.egg-info/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1795 2023-06-18 06:11:03.000000 django-mcq-0.4/django_mcq.egg-info/PKG-INFO
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1183 2023-06-18 06:11:03.000000 django-mcq-0.4/django_mcq.egg-info/SOURCES.txt
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)        1 2023-06-18 06:11:03.000000 django-mcq-0.4/django_mcq.egg-info/dependency_links.txt
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)        1 2023-05-01 02:49:00.000000 django-mcq-0.4/django_mcq.egg-info/not-zip-safe
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)       14 2023-06-18 06:11:03.000000 django-mcq-0.4/django_mcq.egg-info/requires.txt
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)        5 2023-06-18 06:11:03.000000 django-mcq-0.4/django_mcq.egg-info/top_level.txt
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      104 2023-05-01 02:01:55.000000 django-mcq-0.4/pyproject.toml
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-06-18 06:11:03.287757 django-mcq-0.4/quiz/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:01:55.000000 django-mcq-0.4/quiz/__init__.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)       63 2023-05-01 02:01:55.000000 django-mcq-0.4/quiz/admin.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      140 2023-05-01 02:01:55.000000 django-mcq-0.4/quiz/apps.py
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-06-18 06:11:03.287757 django-mcq-0.4/quiz/fixtures/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)    16766 2023-05-01 02:01:55.000000 django-mcq-0.4/quiz/fixtures/sample_quizzes.json
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      879 2023-05-01 02:01:55.000000 django-mcq-0.4/quiz/forms.py
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-06-18 06:11:03.291757 django-mcq-0.4/quiz/migrations/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     6373 2023-05-01 02:01:55.000000 django-mcq-0.4/quiz/migrations/0001_initial.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      718 2023-06-18 05:39:19.000000 django-mcq-0.4/quiz/migrations/0002_answer_img_question_img_question_img_explanation.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:01:55.000000 django-mcq-0.4/quiz/migrations/__init__.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     3200 2023-06-18 05:39:19.000000 django-mcq-0.4/quiz/models.py
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-06-18 06:11:03.279758 django-mcq-0.4/quiz/static/
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-06-18 06:11:03.291757 django-mcq-0.4/quiz/static/datatables/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     5222 2023-05-01 02:01:55.000000 django-mcq-0.4/quiz/static/datatables/dataTables.bootstrap4.min.css
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     2085 2023-05-01 02:01:55.000000 django-mcq-0.4/quiz/static/datatables/dataTables.bootstrap4.min.js
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)    82411 2023-05-01 02:01:55.000000 django-mcq-0.4/quiz/static/datatables/jquery.dataTables.min.js
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-06-18 06:11:03.295757 django-mcq-0.4/quiz/static/quiz/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      533 2023-05-01 02:01:55.000000 django-mcq-0.4/quiz/static/quiz/app.css
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)   141997 2023-05-01 02:01:55.000000 django-mcq-0.4/quiz/static/quiz/bootstrap.min.css
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)    86927 2023-05-01 02:01:55.000000 django-mcq-0.4/quiz/static/quiz/jquery-3.3.1.min.js
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-06-18 06:11:03.279758 django-mcq-0.4/quiz/templates/
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-06-18 06:11:03.299757 django-mcq-0.4/quiz/templates/quiz/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      670 2023-05-01 02:01:55.000000 django-mcq-0.4/quiz/templates/quiz/_header.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      801 2023-05-01 02:01:55.000000 django-mcq-0.4/quiz/templates/quiz/base.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      384 2023-05-01 02:01:55.000000 django-mcq-0.4/quiz/templates/quiz/interests_form.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     3591 2023-06-18 05:39:19.000000 django-mcq-0.4/quiz/templates/quiz/quiz_list.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1997 2023-06-18 05:39:19.000000 django-mcq-0.4/quiz/templates/quiz/quiz_result.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1251 2023-05-01 02:01:55.000000 django-mcq-0.4/quiz/templates/quiz/student_detail.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     2396 2023-05-01 02:01:55.000000 django-mcq-0.4/quiz/templates/quiz/student_list.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      836 2023-06-18 05:39:19.000000 django-mcq-0.4/quiz/templates/quiz/take_quiz_form.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      847 2023-05-01 02:01:55.000000 django-mcq-0.4/quiz/templates/quiz/taken_quiz_list.html
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-06-18 06:11:03.299757 django-mcq-0.4/quiz/templatetags/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:01:55.000000 django-mcq-0.4/quiz/templatetags/__init__.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      995 2023-05-01 02:01:55.000000 django-mcq-0.4/quiz/templatetags/quiz_extras.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)       60 2023-05-01 02:01:55.000000 django-mcq-0.4/quiz/tests.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      724 2023-05-14 04:12:39.000000 django-mcq-0.4/quiz/urls.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     8143 2023-06-18 05:39:19.000000 django-mcq-0.4/quiz/views.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)       38 2023-06-18 06:11:03.303757 django-mcq-0.4/setup.cfg
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1078 2023-06-18 06:09:56.000000 django-mcq-0.4/setup.py
```

### Comparing `django-mcq-0.3/LICENSE` & `django-mcq-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mcq-0.3/PKG-INFO` & `django-mcq-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mcq
-Version: 0.3
+Version: 0.4
 Summary: A configurable quiz app for Django.
 Home-page: https://github.com/suhailvs/django-mcq
 Author: Suhail VS
 Author-email: suhailvs@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-mcq Version: 0.3 Summary: A configurable
+Metadata-Version: 2.1 Name: django-mcq Version: 0.4 Summary: A configurable
 quiz app for Django. Home-page: https://github.com/suhailvs/django-mcq Author:
 Suhail VS Author-email: suhailvs@gmail.com License: MIT License Classifier:
 Environment :: Web Environment Classifier: Framework :: Django Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Internet
```

### Comparing `django-mcq-0.3/README.md` & `django-mcq-0.4/README.md`

 * *Files identical despite different names*

### Comparing `django-mcq-0.3/django_mcq.egg-info/PKG-INFO` & `django-mcq-0.4/django_mcq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mcq
-Version: 0.3
+Version: 0.4
 Summary: A configurable quiz app for Django.
 Home-page: https://github.com/suhailvs/django-mcq
 Author: Suhail VS
 Author-email: suhailvs@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-mcq Version: 0.3 Summary: A configurable
+Metadata-Version: 2.1 Name: django-mcq Version: 0.4 Summary: A configurable
 quiz app for Django. Home-page: https://github.com/suhailvs/django-mcq Author:
 Suhail VS Author-email: suhailvs@gmail.com License: MIT License Classifier:
 Environment :: Web Environment Classifier: Framework :: Django Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Internet
```

### Comparing `django-mcq-0.3/django_mcq.egg-info/SOURCES.txt` & `django-mcq-0.4/django_mcq.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 quiz/forms.py
 quiz/models.py
 quiz/tests.py
 quiz/urls.py
 quiz/views.py
 quiz/fixtures/sample_quizzes.json
 quiz/migrations/0001_initial.py
+quiz/migrations/0002_answer_img_question_img_question_img_explanation.py
 quiz/migrations/__init__.py
 quiz/static/datatables/dataTables.bootstrap4.min.css
 quiz/static/datatables/dataTables.bootstrap4.min.js
 quiz/static/datatables/jquery.dataTables.min.js
 quiz/static/quiz/app.css
 quiz/static/quiz/bootstrap.min.css
 quiz/static/quiz/jquery-3.3.1.min.js
```

### Comparing `django-mcq-0.3/quiz/fixtures/sample_quizzes.json` & `django-mcq-0.4/quiz/fixtures/sample_quizzes.json`

 * *Files identical despite different names*

### Comparing `django-mcq-0.3/quiz/forms.py` & `django-mcq-0.4/quiz/forms.py`

 * *Files identical despite different names*

### Comparing `django-mcq-0.3/quiz/migrations/0001_initial.py` & `django-mcq-0.4/quiz/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mcq-0.3/quiz/models.py` & `django-mcq-0.4/quiz/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from django.db import models
-from django.utils.html import escape, mark_safe
+from django.utils.html import escape, mark_safe, format_html
 # Create your models here.
 from django.conf import settings
+from django.templatetags.static import static
 
 class Subject(models.Model):
     name = models.CharField(max_length=30)
     color = models.CharField(max_length=7, default='#007bff')
 
     def __str__(self):
         return self.name
@@ -25,26 +26,34 @@
     def __str__(self):
         return self.name
 
 
 class Question(models.Model):
     quiz = models.ForeignKey(Quiz, on_delete=models.CASCADE, related_name='questions')
     text = models.TextField('Question')
-
+    img = models.CharField(max_length=250, blank=True)
+    img_explanation = models.CharField(max_length=250, blank=True)
     def __str__(self):
         return self.text
 
 
 class Answer(models.Model):
     question = models.ForeignKey(Question, on_delete=models.CASCADE, related_name='answers')
     text = models.CharField('Answer', max_length=255)
+    img = models.CharField(max_length=250, blank=True)
     is_correct = models.BooleanField('Correct answer', default=False)
 
     def __str__(self):
-        return self.text
+        image_url = ''
+        str_html = f'<span style="cursor:pointer">{self.text}'
+        if self.img:
+            image_url = static(f'quiz_img/{self.img}')
+            str_html += '<br><img src="{}" class="img-thumbnail" style="max-width: 100%"><hr>'
+        str_html += '</span>'
+        return format_html(str_html, image_url)
 
 
 class Student(models.Model):
     user = models.OneToOneField(settings.AUTH_USER_MODEL, on_delete=models.CASCADE, primary_key=True)
     quizzes = models.ManyToManyField(Quiz, through='TakenQuiz')
     interests = models.ManyToManyField(Subject, related_name='interested_students')
```

### Comparing `django-mcq-0.3/quiz/static/datatables/dataTables.bootstrap4.min.css` & `django-mcq-0.4/quiz/static/datatables/dataTables.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `django-mcq-0.3/quiz/static/datatables/dataTables.bootstrap4.min.js` & `django-mcq-0.4/quiz/static/datatables/dataTables.bootstrap4.min.js`

 * *Files identical despite different names*

### Comparing `django-mcq-0.3/quiz/static/datatables/jquery.dataTables.min.js` & `django-mcq-0.4/quiz/static/datatables/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `django-mcq-0.3/quiz/static/quiz/app.css` & `django-mcq-0.4/quiz/static/quiz/app.css`

 * *Files identical despite different names*

### Comparing `django-mcq-0.3/quiz/static/quiz/bootstrap.min.css` & `django-mcq-0.4/quiz/static/quiz/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-mcq-0.3/quiz/static/quiz/jquery-3.3.1.min.js` & `django-mcq-0.4/quiz/static/quiz/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `django-mcq-0.3/quiz/templates/quiz/_header.html` & `django-mcq-0.4/quiz/templates/quiz/_header.html`

 * *Files identical despite different names*

### Comparing `django-mcq-0.3/quiz/templates/quiz/base.html` & `django-mcq-0.4/quiz/templates/quiz/base.html`

 * *Files identical despite different names*

### Comparing `django-mcq-0.3/quiz/templates/quiz/quiz_list.html` & `django-mcq-0.4/quiz/templates/quiz/quiz_list.html`

 * *Files 7% similar despite different names*

```diff
@@ -21,19 +21,21 @@
           <div class="form-group">
             
             <label>Quizzes as JSON</label>
             <textarea class="form-control" id="txt_quizzes_json" rows="10"></textarea>
             <label>Example JSON</label>
             <pre><code>
 [{
-  "quiz": "World War 1", "subject": "History", "questions": [
+  "quiz": "Physics Plus One", "subject": "Physics", "questions": [
       {
-          "question":"When was the Treaty of Versailles signed?",
+          "question":"How many atoms in the cube?",
+          "img":"plus2_chap1/1_e1_quest.jpg",
+          "img_explanation":"plus2_chap1/1_e1_sol.jpg",
           "answers":[
-              {"answer":"June 29 of 1919", "is_correct": "true"}
+              {"answer":"", "is_correct": "true", "img":"plus2_chap1/1_e1_ans1.jpg"}
           ]
       }
   ]
 }]
               </code></pre>
           </div>
           <div id="quizzes_result"></div>
```

### Comparing `django-mcq-0.3/quiz/templates/quiz/quiz_result.html` & `django-mcq-0.4/quiz/templates/quiz/student_detail.html`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,37 @@
 {% extends 'quiz/base.html' %}
+{% load static %}
 {% load quiz_extras %}
 
 {% block content %}
-{% include 'quiz/_header.html' with active='taken' %}
+{% include 'quiz/_header.html' with active='profile' %}
 <nav aria-label="breadcrumb">
     <ol class="breadcrumb">
-      <li class="breadcrumb-item"><a href="{% url 'quiz:taken_quiz_list' %}">Quizzes</a></li>
-      <li class="breadcrumb-item active" aria-current="page">{{quiz.name}}</li>
+      <li class="breadcrumb-item"><a href="{% url 'quiz:student_list' %}">Students</a></li>
+      <li class="breadcrumb-item active" aria-current="page">{{student.user.username}}</li>
     </ol>
 </nav>
-<!-- <h2>{{quiz.name}}</h2> -->
-{{ quiz.subject.get_html_badge }}
-
-<div class="progress">
-  <div class="progress-bar progress-bar-striped bg-success" role="progressbar" style="width: {{percentage}}%" aria-valuenow="{{percentage}}" aria-valuemin="0" aria-valuemax="100">{{percentage}}%</div>
-</div><br>
-{% for question in questions %}
-<div class="card">
-  <div class="card-body">
-    <h5 class="card-title">{{forloop.counter}}. {{question.text}}</h5>
-    <table class="table table-bordered table-sm">
-      <thead><tr><th>Yours</th><th>Correct</th><th></th></tr></thead>
+<div class="row">
+  <div class="col-md-4">
+      <img class="img-thumbnail" src="{{ student.user.email|gravatar_url:200 }}" width="200" height="200" alt="@{{ student.user.email}}">
+  </div>
+  <div class="col-md-8">
+  	<div class="card">
+    <table class="table mb-0">
+      
       <tbody>
-        {% for opt in question.answers.all %}
-        {% marked_answer user opt as opt_marked %}        
-        <tr>
-          <td style="width: 100px;{% if opt_marked == 'correct' %} background:green{% elif opt_marked == 'wrong' %} background:red{% endif %}"> </td>
-          <td style="width: 100px;{% if opt.is_correct %} background:green{% endif %}"></td>
-          <td>{{opt.text}}</td>
-        </tr>
-        {% endfor %}
+      	<tr><td>Email</td><td>{{student.user.email}}</td></tr>
+      	<tr><td>Username</td><td>{{student.user.username}}</td></tr>
+      	<tr><td>Fullname</td><td>{{student.user.get_full_name}}</td></tr>
+      	<tr><td>POINTS</td><td>{{student.score}}</td></tr>
       </tbody>
     </table>
+	</div>
   </div>
-</div>
-<br>
+</div><hr>
+<h3>Top Subjects</h3>
+{% for subject in subjects %}
+	<span class="badge badge-primary" style="background-color:{{subject.quiz__subject__color}}">
+		{{subject.quiz__subject__name}}
+	</span> x {{subject.score}}
 {% endfor %}
 {% endblock %}
-
-{% block js %}
-<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
-<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
-{% endblock %}
```

#### html2text {}

```diff
@@ -1,14 +1,13 @@
-{% extends 'quiz/base.html' %} {% load quiz_extras %} {% block content %} {%
-include 'quiz/_header.html' with active='taken' %}
-   1. Quizzes
-   2. {{quiz.name}}
-  {{ quiz.subject.get_html_badge }}
-{{percentage}}%
-
-{% for question in questions %}
-** {{forloop.counter}}. {{question.text}} **
-Yours Correct
-              {{opt.text}}
-
-{% endfor %} {% endblock %} {% block js %}
- {% endblock %}
+{% extends 'quiz/base.html' %} {% load static %} {% load quiz_extras %} {%
+block content %} {% include 'quiz/_header.html' with active='profile' %}
+   1. Students
+   2. {{student.user.username}}
+[@{{ student.user.email}}]
+Email    {{student.user.email}}
+Username {{student.user.username}}
+Fullname {{student.user.get_full_name}}
+POINTS   {{student.score}}
+===============================================================================
+**** Top Subjects ****
+{% for subject in subjects %}  {{subject.quiz__subject__name}}  x {
+{subject.score}} {% endfor %} {% endblock %}
```

### Comparing `django-mcq-0.3/quiz/templates/quiz/student_list.html` & `django-mcq-0.4/quiz/templates/quiz/student_list.html`

 * *Files identical despite different names*

### Comparing `django-mcq-0.3/quiz/templates/quiz/take_quiz_form.html` & `django-mcq-0.4/quiz/templates/quiz/take_quiz_form.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 {% extends 'quiz/base.html' %}
 
 {# load crispy_forms_tags #}
-
+{% load static %}
 
 {% block content %}
 {% include 'quiz/_header.html' with active='new' %}
   <div class="progress mb-3">
     <div class="progress-bar" role="progressbar" aria-valuenow="{{ progress }}" aria-valuemin="0" aria-valuemax="100" style="width: {{ progress }}%"></div>
   </div>
   <h2><span class="badge badge-secondary">{{ answered_questions|add:"1" }}/{{total_questions}}</span></h2>
   
   <h2 class="mb-3">{{ quiz.name }}</h2>
   <p class="lead">{{ question.text }}</p>
+  {% if question.img %}<img src="{% static 'quiz_img/'|add:question.img %}" class="img-thumbnail" style="max-width: 100%">{% endif %}
   <form method="post" novalidate>
     {% csrf_token %}
     {{ form }}
     <button type="submit" class="btn btn-primary">Next →</button>
   </form>
 {% endblock %}
```

### Comparing `django-mcq-0.3/quiz/templates/quiz/taken_quiz_list.html` & `django-mcq-0.4/quiz/templates/quiz/taken_quiz_list.html`

 * *Files identical despite different names*

### Comparing `django-mcq-0.3/quiz/templatetags/quiz_extras.py` & `django-mcq-0.4/quiz/templatetags/quiz_extras.py`

 * *Files identical despite different names*

### Comparing `django-mcq-0.3/quiz/urls.py` & `django-mcq-0.4/quiz/urls.py`

 * *Files identical despite different names*

### Comparing `django-mcq-0.3/quiz/views.py` & `django-mcq-0.4/quiz/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,18 +83,19 @@
 
 @method_decorator([login_required], name='dispatch')
 class CreateQuizView(View):
     def create_quiz(self, quiz):
         subject, _ = Subject.objects.get_or_create(name=quiz['subject'])
         quiz_item= Quiz.objects.create(name=quiz['quiz'],subject=subject)
         for question in quiz['questions']:
-            question_item = Question.objects.create(quiz=quiz_item,text=question['question'])
+            question_item = Question.objects.create(quiz=quiz_item,text=question['question'], 
+                img = question['img'],img_explanation = question['img_explanation'])
             for answer in question['answers']:
                 is_correct = True if answer['is_correct'] == 'true' else False
-                Answer.objects.create(question = question_item, text = answer['answer'],is_correct=is_correct)
+                Answer.objects.create(question = question_item, text = answer['answer'],is_correct=is_correct, img = answer['img'])
     def post(self, request, *args, **kwargs): 
         import json
         try:
             quizzes = json.loads(request.POST['txt_quizzes_json'])
             with transaction.atomic():
                 for quiz in quizzes:
                     self.create_quiz(quiz)
```

### Comparing `django-mcq-0.3/setup.py` & `django-mcq-0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 readme = open('README.md', encoding='utf-8')
 long_description = readme.read()
 
 
 setup(
     name='django-mcq',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
     include_package_data=True,
     license='MIT License',
     description='A configurable quiz app for Django.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/suhailvs/django-mcq',
```

