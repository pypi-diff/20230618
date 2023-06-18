# Comparing `tmp/forecastmanager-0.0.1.tar.gz` & `tmp/forecastmanager-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forecastmanager-0.0.1.tar", last modified: Sun Jun 18 17:31:17 2023, max compression
+gzip compressed data, was "forecastmanager-0.0.2.tar", last modified: Sun Jun 18 18:36:58 2023, max compression
```

## Comparing `forecastmanager-0.0.1.tar` & `forecastmanager-0.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:31:17.481536 forecastmanager-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-18 17:31:02.000000 forecastmanager-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-18 17:31:17.481536 forecastmanager-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 17:31:02.000000 forecastmanager-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:31:17.481536 forecastmanager-0.0.1/forecastmanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 17:31:02.000000 forecastmanager-0.0.1/forecastmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-18 17:31:02.000000 forecastmanager-0.0.1/forecastmanager/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-18 17:31:02.000000 forecastmanager-0.0.1/forecastmanager/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:31:17.481536 forecastmanager-0.0.1/forecastmanager/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 17:31:02.000000 forecastmanager-0.0.1/forecastmanager/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:31:17.481536 forecastmanager-0.0.1/forecastmanager/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 17:31:02.000000 forecastmanager-0.0.1/forecastmanager/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-18 17:31:02.000000 forecastmanager-0.0.1/forecastmanager/management/commands/generate_forecast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:31:17.481536 forecastmanager-0.0.1/forecastmanager/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-18 17:31:02.000000 forecastmanager-0.0.1/forecastmanager/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 17:31:02.000000 forecastmanager-0.0.1/forecastmanager/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-18 17:31:02.000000 forecastmanager-0.0.1/forecastmanager/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-18 17:31:02.000000 forecastmanager-0.0.1/forecastmanager/site_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:31:17.477536 forecastmanager-0.0.1/forecastmanager/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:31:17.481536 forecastmanager-0.0.1/forecastmanager/templates/forecastmanager/
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-18 17:31:02.000000 forecastmanager-0.0.1/forecastmanager/templates/forecastmanager/create_forecast.html
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-18 17:31:02.000000 forecastmanager-0.0.1/forecastmanager/templates/forecastmanager/forecast.html
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-18 17:31:02.000000 forecastmanager-0.0.1/forecastmanager/templates/forecastmanager/query_forecast.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-18 17:31:02.000000 forecastmanager-0.0.1/forecastmanager/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-18 17:31:02.000000 forecastmanager-0.0.1/forecastmanager/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-18 17:31:02.000000 forecastmanager-0.0.1/forecastmanager/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:31:17.481536 forecastmanager-0.0.1/forecastmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-18 17:31:17.000000 forecastmanager-0.0.1/forecastmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-18 17:31:17.000000 forecastmanager-0.0.1/forecastmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 17:31:17.000000 forecastmanager-0.0.1/forecastmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-18 17:31:17.000000 forecastmanager-0.0.1/forecastmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-18 17:31:17.000000 forecastmanager-0.0.1/forecastmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-18 17:31:02.000000 forecastmanager-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-18 17:31:17.481536 forecastmanager-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:58.096684 forecastmanager-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-18 18:36:58.096684 forecastmanager-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:58.096684 forecastmanager-0.0.2/forecastmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:58.096684 forecastmanager-0.0.2/forecastmanager/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:58.096684 forecastmanager-0.0.2/forecastmanager/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/management/commands/generate_forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:58.096684 forecastmanager-0.0.2/forecastmanager/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/site_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:58.096684 forecastmanager-0.0.2/forecastmanager/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:58.096684 forecastmanager-0.0.2/forecastmanager/templates/forecastmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/templates/forecastmanager/create_forecast.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/templates/forecastmanager/forecast.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/templates/forecastmanager/query_forecast.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/forecastmanager/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:36:58.096684 forecastmanager-0.0.2/forecastmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-18 18:36:58.000000 forecastmanager-0.0.2/forecastmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-18 18:36:58.000000 forecastmanager-0.0.2/forecastmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 18:36:58.000000 forecastmanager-0.0.2/forecastmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-18 18:36:58.000000 forecastmanager-0.0.2/forecastmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-18 18:36:58.000000 forecastmanager-0.0.2/forecastmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-18 18:36:43.000000 forecastmanager-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-18 18:36:58.096684 forecastmanager-0.0.2/setup.cfg
```

### Comparing `forecastmanager-0.0.1/PKG-INFO` & `forecastmanager-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecastmanager
-Version: 0.0.1
+Version: 0.0.2
 Summary: Integration of Weather City Forecasts Manager in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/forecastmanager
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `forecastmanager-0.0.1/forecastmanager/management/commands/generate_forecast.py` & `forecastmanager-0.0.2/forecastmanager/management/commands/generate_forecast.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.1/forecastmanager/migrations/0001_initial.py` & `forecastmanager-0.0.2/forecastmanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.1/forecastmanager/models.py` & `forecastmanager-0.0.2/forecastmanager/models.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.1/forecastmanager/site_settings.py` & `forecastmanager-0.0.2/forecastmanager/site_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 from wagtail.admin.panels import (
     FieldPanel,
     TabbedInterface,
     ObjectList,
 )
-@register_setting
+# @register_setting
 class Setting(BaseSiteSetting):
     enable_auto_forecast = models.BooleanField(
         default=True,
         verbose_name=_('Enable automated forecasts')
     )
 
     TEMPERATURE_UNITS = (
```

### Comparing `forecastmanager-0.0.1/forecastmanager/templates/forecastmanager/create_forecast.html` & `forecastmanager-0.0.2/forecastmanager/templates/forecastmanager/create_forecast.html`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.1/forecastmanager/templates/forecastmanager/forecast.html` & `forecastmanager-0.0.2/forecastmanager/templates/forecastmanager/forecast.html`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 {% endblock extra_js %}
 
 
 {% block content %}
 
 <div class="messages" role="status">
     <ul>
-        {% if settings.base.IntegrationSettings.enable_auto_forecast %}
+        {% if settings.forecastmanager.Setting.enable_auto_forecast %}
         <li class="warning">                            
             <svg class="icon icon-warning messages-icon" aria-hidden="true"><use href="#icon-warning"></use></svg>
             Autoforecasting has been enabled and manually added forecasts here will be overidden.
             <span class="buttons">
                 <a href="/admin/settings/forecastmanager/setting" class="button button-small button-secondary">Change autoforecasting setting</a>
             </span>
         </li>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 {% extends "wagtailadmin/base.html" %} {% load wagtailadmin_tags i18n static %}
 {% block extra_css %} {{ block.super }} {% comment %}
  {% endcomment %}
  {{ form.media.css }} {% endblock %} {% block titletag %} {% trans 'Forecast
 Manager' %} {% endblock %} {% block extra_js %} {{block.super}} {% include
 "wagtailadmin/pages/_editor_js.html" %} {{ form.media.js}}
  {% endblock extra_js %} {% block content %}
-    * {% if settings.base.IntegrationSettings.enable_auto_forecast %}
+    * {% if settings.forecastmanager.Setting.enable_auto_forecast %}
     *  Autoforecasting has been enabled and manually added forecasts here will
       be overidden.  Change_autoforecasting_setting
     * {% endif %}
     *    Data Saved Successfuly
     *
 {% trans 'Forecast Manager' as title_str %} {% include "wagtailadmin/shared/
 header.html" with title=title_str icon='form' %} {% include "wagtailadmin/
```

### Comparing `forecastmanager-0.0.1/forecastmanager/templates/forecastmanager/query_forecast.html` & `forecastmanager-0.0.2/forecastmanager/templates/forecastmanager/query_forecast.html`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.1/forecastmanager/views.py` & `forecastmanager-0.0.2/forecastmanager/views.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.1/forecastmanager/wagtail_hooks.py` & `forecastmanager-0.0.2/forecastmanager/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.1/forecastmanager.egg-info/PKG-INFO` & `forecastmanager-0.0.2/forecastmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecastmanager
-Version: 0.0.1
+Version: 0.0.2
 Summary: Integration of Weather City Forecasts Manager in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/forecastmanager
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `forecastmanager-0.0.1/forecastmanager.egg-info/SOURCES.txt` & `forecastmanager-0.0.2/forecastmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.1/setup.cfg` & `forecastmanager-0.0.2/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = forecastmanager
-version = 0.0.1
+version = 0.0.2
 description = Integration of Weather City Forecasts Manager in Wagtail Projects.
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/forecastmanager
 author = Grace Amondi
 author_email = miswa.grace@gmail.com
 license = MIT
```

