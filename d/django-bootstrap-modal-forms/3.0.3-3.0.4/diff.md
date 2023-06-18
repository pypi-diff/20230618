# Comparing `tmp/django-bootstrap-modal-forms-3.0.3.tar.gz` & `tmp/django-bootstrap-modal-forms-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-bootstrap-modal-forms-3.0.3.tar", last modified: Sun Jun  4 16:54:03 2023, max compression
+gzip compressed data, was "django-bootstrap-modal-forms-3.0.4.tar", last modified: Sun Jun 18 13:54:03 2023, max compression
```

## Comparing `django-bootstrap-modal-forms-3.0.3.tar` & `django-bootstrap-modal-forms-3.0.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:54:03.455512 django-bootstrap-modal-forms-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    37063 2023-06-04 16:54:03.455512 django-bootstrap-modal-forms-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36236 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:54:03.447512 django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:54:03.439513 django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:54:03.447512 django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.js
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.js
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:54:03.447512 django-bootstrap-modal-forms-3.0.3/django_bootstrap_modal_forms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37063 2023-06-04 16:54:03.000000 django-bootstrap-modal-forms-3.0.3/django_bootstrap_modal_forms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-04 16:54:03.000000 django-bootstrap-modal-forms-3.0.3/django_bootstrap_modal_forms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 16:54:03.000000 django-bootstrap-modal-forms-3.0.3/django_bootstrap_modal_forms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 16:54:03.000000 django-bootstrap-modal-forms-3.0.3/django_bootstrap_modal_forms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-04 16:54:03.000000 django-bootstrap-modal-forms-3.0.3/django_bootstrap_modal_forms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:54:03.451512 django-bootstrap-modal-forms-3.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/examples/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/examples/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:54:03.451512 django-bootstrap-modal-forms-3.0.3/examples/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/examples/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/examples/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/examples/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/examples/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/examples/views.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:54:03.451512 django-bootstrap-modal-forms-3.0.3/setup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/setup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/setup/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/setup/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/setup/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 16:54:03.455512 django-bootstrap-modal-forms-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:54:03.451512 django-bootstrap-modal-forms-3.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/tests/tests_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/tests/tests_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:54:03.522865 django-bootstrap-modal-forms-3.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    37063 2023-06-18 13:54:03.522865 django-bootstrap-modal-forms-3.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36236 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:54:03.518865 django-bootstrap-modal-forms-3.0.4/bootstrap_modal_forms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/bootstrap_modal_forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/bootstrap_modal_forms/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/bootstrap_modal_forms/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/bootstrap_modal_forms/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:54:03.514865 django-bootstrap-modal-forms-3.0.4/bootstrap_modal_forms/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:54:03.518865 django-bootstrap-modal-forms-3.0.4/bootstrap_modal_forms/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:54:03.518865 django-bootstrap-modal-forms-3.0.4/django_bootstrap_modal_forms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37063 2023-06-18 13:54:03.000000 django-bootstrap-modal-forms-3.0.4/django_bootstrap_modal_forms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-18 13:54:03.000000 django-bootstrap-modal-forms-3.0.4/django_bootstrap_modal_forms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 13:54:03.000000 django-bootstrap-modal-forms-3.0.4/django_bootstrap_modal_forms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 13:54:03.000000 django-bootstrap-modal-forms-3.0.4/django_bootstrap_modal_forms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-18 13:54:03.000000 django-bootstrap-modal-forms-3.0.4/django_bootstrap_modal_forms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:54:03.518865 django-bootstrap-modal-forms-3.0.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/examples/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/examples/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:54:03.518865 django-bootstrap-modal-forms-3.0.4/examples/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/examples/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/examples/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/examples/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/examples/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/examples/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:54:03.522865 django-bootstrap-modal-forms-3.0.4/setup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/setup/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/setup/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/setup/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 13:54:03.522865 django-bootstrap-modal-forms-3.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:54:03.522865 django-bootstrap-modal-forms-3.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/tests/tests_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-06-18 13:53:54.000000 django-bootstrap-modal-forms-3.0.4/tests/tests_unit.py
```

### Comparing `django-bootstrap-modal-forms-3.0.3/CHANGELOG.rst` & `django-bootstrap-modal-forms-3.0.4/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 =========
 Changelog
 =========
 
+3.0.4 (2023-06-18)
+==================
+
+- fix broken examples by bumping django-widget-tweaks dependency version
+
+3.0.3 (2023-06-04)
+==================
+
+- add get_success_message method in FormValidationMixin
+
+
 3.0.2 (2023-05-02)
 ==================
 
 - fix call to get_success_url method in FormValidationMixin
 
 3.0.1 (2023-05-02)
 ==================
```

### Comparing `django-bootstrap-modal-forms-3.0.3/LICENSE.txt` & `django-bootstrap-modal-forms-3.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.3/PKG-INFO` & `django-bootstrap-modal-forms-3.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bootstrap-modal-forms
-Version: 3.0.3
+Version: 3.0.4
 Summary: A Django plugin for creating AJAX driven forms in Bootstrap modal.
 Home-page: https://github.com/trco/django-bootstrap-modal-forms
 Author: Uros Trstenjak
 Author-email: uros.trstenjak@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `django-bootstrap-modal-forms-3.0.3/README.rst` & `django-bootstrap-modal-forms-3.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/generic.py` & `django-bootstrap-modal-forms-3.0.4/bootstrap_modal_forms/generic.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/mixins.py` & `django-bootstrap-modal-forms-3.0.4/bootstrap_modal_forms/mixins.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.js` & `django-bootstrap-modal-forms-3.0.4/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 /*
 django-bootstrap-modal-forms
-version : 3.0.3
+version : 3.0.4
 Copyright (c) 2023 Marcel Rupp
 */
 
 // Open modal & load the form at formURL to the modalContent element
 const modalFormCallback = function(settings) {
     let modal = document.querySelector(settings.modalID);
     let content = modal.querySelector(settings.modalContent);
```

### Comparing `django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.min.js` & `django-bootstrap-modal-forms-3.0.4/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.min.js`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.js` & `django-bootstrap-modal-forms-3.0.4/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 /*
 django-bootstrap-modal-forms
-version : 3.0.3
+version : 3.0.4
 Copyright (c) 2023 Uroš Trstenjak
 https://github.com/trco/django-bootstrap-modal-forms
 */
 
 (function($) {
 
     // Open modal & load the form at formURL to the modalContent element
```

### Comparing `django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.min.js` & `django-bootstrap-modal-forms-3.0.4/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.min.js`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.3/django_bootstrap_modal_forms.egg-info/PKG-INFO` & `django-bootstrap-modal-forms-3.0.4/django_bootstrap_modal_forms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bootstrap-modal-forms
-Version: 3.0.3
+Version: 3.0.4
 Summary: A Django plugin for creating AJAX driven forms in Bootstrap modal.
 Home-page: https://github.com/trco/django-bootstrap-modal-forms
 Author: Uros Trstenjak
 Author-email: uros.trstenjak@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `django-bootstrap-modal-forms-3.0.3/django_bootstrap_modal_forms.egg-info/SOURCES.txt` & `django-bootstrap-modal-forms-3.0.4/django_bootstrap_modal_forms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.3/examples/forms.py` & `django-bootstrap-modal-forms-3.0.4/examples/forms.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.3/examples/migrations/0001_initial.py` & `django-bootstrap-modal-forms-3.0.4/examples/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.3/examples/models.py` & `django-bootstrap-modal-forms-3.0.4/examples/models.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.3/examples/urls.py` & `django-bootstrap-modal-forms-3.0.4/examples/urls.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.3/examples/views.py` & `django-bootstrap-modal-forms-3.0.4/examples/views.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.3/setup/settings.py` & `django-bootstrap-modal-forms-3.0.4/setup/settings.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.3/setup.py` & `django-bootstrap-modal-forms-3.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     README = readme_file.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-bootstrap-modal-forms',
-    version='3.0.3',
+    version='3.0.4',
     packages=find_packages(),
     include_package_data=True,
     license='MIT License',
     description='A Django plugin for creating AJAX driven forms in Bootstrap modal.',
     long_description=README,
     url='https://github.com/trco/django-bootstrap-modal-forms',
     author='Uros Trstenjak',
```

### Comparing `django-bootstrap-modal-forms-3.0.3/tests/base.py` & `django-bootstrap-modal-forms-3.0.4/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.3/tests/tests_functional.py` & `django-bootstrap-modal-forms-3.0.4/tests/tests_functional.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.3/tests/tests_unit.py` & `django-bootstrap-modal-forms-3.0.4/tests/tests_unit.py`

 * *Files identical despite different names*

