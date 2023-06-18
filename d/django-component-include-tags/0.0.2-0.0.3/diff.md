# Comparing `tmp/django_component_include_tags-0.0.2.tar.gz` & `tmp/django_component_include_tags-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_component_include_tags-0.0.2.tar", last modified: Sun Jun 18 16:46:10 2023, max compression
+gzip compressed data, was "django_component_include_tags-0.0.3.tar", last modified: Sun Jun 18 17:12:48 2023, max compression
```

## Comparing `django_component_include_tags-0.0.2.tar` & `django_component_include_tags-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 redmond   (1000) redmond   (1000)        0 2023-06-18 16:46:10.055271 django_component_include_tags-0.0.2/
--rw-r--r--   0 redmond   (1000) redmond   (1000)     1061 2023-06-18 15:36:39.000000 django_component_include_tags-0.0.2/LICENCE
--rw-r--r--   0 redmond   (1000) redmond   (1000)     4777 2023-06-18 16:46:10.055271 django_component_include_tags-0.0.2/PKG-INFO
--rw-r--r--   0 redmond   (1000) redmond   (1000)     4187 2023-06-18 15:49:33.000000 django_component_include_tags-0.0.2/README.md
--rw-r--r--   0 redmond   (1000) redmond   (1000)      716 2023-06-18 16:46:06.000000 django_component_include_tags-0.0.2/pyproject.toml
--rw-r--r--   0 redmond   (1000) redmond   (1000)       38 2023-06-18 16:46:10.055271 django_component_include_tags-0.0.2/setup.cfg
-drwxr-xr-x   0 redmond   (1000) redmond   (1000)        0 2023-06-18 16:46:10.045272 django_component_include_tags-0.0.2/src/
-drwxr-xr-x   0 redmond   (1000) redmond   (1000)        0 2023-06-18 16:46:10.055271 django_component_include_tags-0.0.2/src/component_include_tags/
--rw-r--r--   0 redmond   (1000) redmond   (1000)        0 2023-06-18 14:15:20.000000 django_component_include_tags-0.0.2/src/component_include_tags/__init__.py
--rw-r--r--   0 redmond   (1000) redmond   (1000)      174 2023-06-18 14:15:20.000000 django_component_include_tags-0.0.2/src/component_include_tags/apps.py
-drwxr-xr-x   0 redmond   (1000) redmond   (1000)        0 2023-06-18 16:46:10.055271 django_component_include_tags-0.0.2/src/component_include_tags/migrations/
--rw-r--r--   0 redmond   (1000) redmond   (1000)        0 2023-06-18 14:15:20.000000 django_component_include_tags-0.0.2/src/component_include_tags/migrations/__init__.py
-drwxr-xr-x   0 redmond   (1000) redmond   (1000)        0 2023-06-18 16:46:10.055271 django_component_include_tags-0.0.2/src/component_include_tags/templatetags/
--rw-r--r--   0 redmond   (1000) redmond   (1000)        0 2023-06-18 14:16:28.000000 django_component_include_tags-0.0.2/src/component_include_tags/templatetags/__init__.py
--rw-r--r--   0 redmond   (1000) redmond   (1000)     3817 2023-06-18 14:38:12.000000 django_component_include_tags-0.0.2/src/component_include_tags/templatetags/components.py
--rw-r--r--   0 redmond   (1000) redmond   (1000)     1176 2023-06-18 14:49:29.000000 django_component_include_tags-0.0.2/src/component_include_tags/tests.py
-drwxr-xr-x   0 redmond   (1000) redmond   (1000)        0 2023-06-18 16:46:10.055271 django_component_include_tags-0.0.2/src/django_component_include_tags.egg-info/
--rw-r--r--   0 redmond   (1000) redmond   (1000)     4777 2023-06-18 16:46:10.000000 django_component_include_tags-0.0.2/src/django_component_include_tags.egg-info/PKG-INFO
--rw-r--r--   0 redmond   (1000) redmond   (1000)      526 2023-06-18 16:46:10.000000 django_component_include_tags-0.0.2/src/django_component_include_tags.egg-info/SOURCES.txt
--rw-r--r--   0 redmond   (1000) redmond   (1000)        1 2023-06-18 16:46:10.000000 django_component_include_tags-0.0.2/src/django_component_include_tags.egg-info/dependency_links.txt
--rw-r--r--   0 redmond   (1000) redmond   (1000)       23 2023-06-18 16:46:10.000000 django_component_include_tags-0.0.2/src/django_component_include_tags.egg-info/top_level.txt
+drwxr-xr-x   0 redmond   (1000) redmond   (1000)        0 2023-06-18 17:12:48.084574 django_component_include_tags-0.0.3/
+-rw-r--r--   0 redmond   (1000) redmond   (1000)     1061 2023-06-18 15:36:39.000000 django_component_include_tags-0.0.3/LICENCE
+-rw-r--r--   0 redmond   (1000) redmond   (1000)     4719 2023-06-18 17:12:48.084574 django_component_include_tags-0.0.3/PKG-INFO
+-rw-r--r--   0 redmond   (1000) redmond   (1000)     4187 2023-06-18 15:49:33.000000 django_component_include_tags-0.0.3/README.md
+-rw-r--r--   0 redmond   (1000) redmond   (1000)      637 2023-06-18 17:10:55.000000 django_component_include_tags-0.0.3/pyproject.toml
+-rw-r--r--   0 redmond   (1000) redmond   (1000)       38 2023-06-18 17:12:48.084574 django_component_include_tags-0.0.3/setup.cfg
+drwxr-xr-x   0 redmond   (1000) redmond   (1000)        0 2023-06-18 17:12:48.084574 django_component_include_tags-0.0.3/src/
+drwxr-xr-x   0 redmond   (1000) redmond   (1000)        0 2023-06-18 17:12:48.084574 django_component_include_tags-0.0.3/src/component_include_tags/
+-rw-r--r--   0 redmond   (1000) redmond   (1000)        0 2023-06-18 14:15:20.000000 django_component_include_tags-0.0.3/src/component_include_tags/__init__.py
+-rw-r--r--   0 redmond   (1000) redmond   (1000)      174 2023-06-18 14:15:20.000000 django_component_include_tags-0.0.3/src/component_include_tags/apps.py
+drwxr-xr-x   0 redmond   (1000) redmond   (1000)        0 2023-06-18 17:12:48.084574 django_component_include_tags-0.0.3/src/component_include_tags/migrations/
+-rw-r--r--   0 redmond   (1000) redmond   (1000)        0 2023-06-18 14:15:20.000000 django_component_include_tags-0.0.3/src/component_include_tags/migrations/__init__.py
+drwxr-xr-x   0 redmond   (1000) redmond   (1000)        0 2023-06-18 17:12:48.084574 django_component_include_tags-0.0.3/src/component_include_tags/templatetags/
+-rw-r--r--   0 redmond   (1000) redmond   (1000)        0 2023-06-18 14:16:28.000000 django_component_include_tags-0.0.3/src/component_include_tags/templatetags/__init__.py
+-rw-r--r--   0 redmond   (1000) redmond   (1000)     3817 2023-06-18 14:38:12.000000 django_component_include_tags-0.0.3/src/component_include_tags/templatetags/components.py
+-rw-r--r--   0 redmond   (1000) redmond   (1000)     1176 2023-06-18 14:49:29.000000 django_component_include_tags-0.0.3/src/component_include_tags/tests.py
+drwxr-xr-x   0 redmond   (1000) redmond   (1000)        0 2023-06-18 17:12:48.084574 django_component_include_tags-0.0.3/src/django_component_include_tags.egg-info/
+-rw-r--r--   0 redmond   (1000) redmond   (1000)     4719 2023-06-18 17:12:48.000000 django_component_include_tags-0.0.3/src/django_component_include_tags.egg-info/PKG-INFO
+-rw-r--r--   0 redmond   (1000) redmond   (1000)      526 2023-06-18 17:12:48.000000 django_component_include_tags-0.0.3/src/django_component_include_tags.egg-info/SOURCES.txt
+-rw-r--r--   0 redmond   (1000) redmond   (1000)        1 2023-06-18 17:12:48.000000 django_component_include_tags-0.0.3/src/django_component_include_tags.egg-info/dependency_links.txt
+-rw-r--r--   0 redmond   (1000) redmond   (1000)       23 2023-06-18 17:12:48.000000 django_component_include_tags-0.0.3/src/django_component_include_tags.egg-info/top_level.txt
```

### Comparing `django_component_include_tags-0.0.2/LICENCE` & `django_component_include_tags-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `django_component_include_tags-0.0.2/PKG-INFO` & `django_component_include_tags-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: django_component_include_tags
-Version: 0.0.2
+Version: 0.0.3
 Summary: Component template tags for Django
-Author-email: Redmond Scales <redmond.j.scales@gmail.com>
 Project-URL: Homepage, https://github.com/redmondscales/django-component-include-tags
 Project-URL: Bug Tracker, https://github.com/redmondscales/django-component-include-tags/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `django_component_include_tags-0.0.2/README.md` & `django_component_include_tags-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `django_component_include_tags-0.0.2/pyproject.toml` & `django_component_include_tags-0.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django_component_include_tags"
-version = "0.0.2"
-authors = [
-  { name="Redmond Scales", email="redmond.j.scales@gmail.com" },
-]
+version = "0.0.3"
 description = "Component template tags for Django"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `django_component_include_tags-0.0.2/src/component_include_tags/templatetags/components.py` & `django_component_include_tags-0.0.3/src/component_include_tags/templatetags/components.py`

 * *Files identical despite different names*

### Comparing `django_component_include_tags-0.0.2/src/component_include_tags/tests.py` & `django_component_include_tags-0.0.3/src/component_include_tags/tests.py`

 * *Files identical despite different names*

### Comparing `django_component_include_tags-0.0.2/src/django_component_include_tags.egg-info/PKG-INFO` & `django_component_include_tags-0.0.3/src/django_component_include_tags.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: django-component-include-tags
-Version: 0.0.2
+Version: 0.0.3
 Summary: Component template tags for Django
-Author-email: Redmond Scales <redmond.j.scales@gmail.com>
 Project-URL: Homepage, https://github.com/redmondscales/django-component-include-tags
 Project-URL: Bug Tracker, https://github.com/redmondscales/django-component-include-tags/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `django_component_include_tags-0.0.2/src/django_component_include_tags.egg-info/SOURCES.txt` & `django_component_include_tags-0.0.3/src/django_component_include_tags.egg-info/SOURCES.txt`

 * *Files identical despite different names*

