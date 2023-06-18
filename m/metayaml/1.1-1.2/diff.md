# Comparing `tmp/metayaml-1.1.tar.gz` & `tmp/metayaml-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metayaml-1.1.tar", last modified: Wed May  3 20:27:37 2023, max compression
+gzip compressed data, was "metayaml-1.2.tar", last modified: Sun Jun 18 17:01:07 2023, max compression
```

## Comparing `metayaml-1.1.tar` & `metayaml-1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 20:27:37.297443 metayaml-1.1/
--rw-rw-rw-   0        0        0     8747 2023-05-03 20:27:37.282523 metayaml-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     8138 2022-11-13 22:01:52.000000 metayaml-1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-03 20:27:37.217939 metayaml-1.1/metayaml/
--rw-rw-rw-   0        0        0       72 2015-04-13 21:12:55.000000 metayaml-1.1/metayaml/__init__.py
--rw-rw-rw-   0        0        0      737 2022-11-13 22:01:52.000000 metayaml-1.1/metayaml/exception.py
--rw-rw-rw-   0        0        0     2485 2023-05-01 23:30:26.000000 metayaml-1.1/metayaml/jinja_eval.py
--rw-rw-rw-   0        0        0    11828 2023-05-01 23:34:29.000000 metayaml-1.1/metayaml/metayaml.py
-drwxrwxrwx   0        0        0        0 2023-05-03 20:27:37.282523 metayaml-1.1/metayaml.egg-info/
--rw-rw-rw-   0        0        0     8747 2023-05-03 20:27:36.000000 metayaml-1.1/metayaml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-03 20:27:37.000000 metayaml-1.1/metayaml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 20:27:36.000000 metayaml-1.1/metayaml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-03 20:27:36.000000 metayaml-1.1/metayaml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-03 20:27:36.000000 metayaml-1.1/metayaml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 20:27:37.297443 metayaml-1.1/setup.cfg
--rw-rw-rw-   0        0        0      822 2023-05-01 23:43:35.000000 metayaml-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:01:07.345117 metayaml-1.2/
+-rw-rw-rw-   0        0        0     8747 2023-06-18 17:01:07.344117 metayaml-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8138 2022-11-13 22:01:52.000000 metayaml-1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-18 17:01:07.338156 metayaml-1.2/metayaml/
+-rw-rw-rw-   0        0        0       72 2015-04-13 21:12:55.000000 metayaml-1.2/metayaml/__init__.py
+-rw-rw-rw-   0        0        0      737 2022-11-13 22:01:52.000000 metayaml-1.2/metayaml/exception.py
+-rw-rw-rw-   0        0        0     2485 2023-05-01 23:30:26.000000 metayaml-1.2/metayaml/jinja_eval.py
+-rw-rw-rw-   0        0        0    11912 2023-06-18 16:19:10.000000 metayaml-1.2/metayaml/metayaml.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:01:07.343116 metayaml-1.2/metayaml.egg-info/
+-rw-rw-rw-   0        0        0     8747 2023-06-18 17:01:07.000000 metayaml-1.2/metayaml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-06-18 17:01:07.000000 metayaml-1.2/metayaml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 17:01:07.000000 metayaml-1.2/metayaml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-18 17:01:07.000000 metayaml-1.2/metayaml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-18 17:01:07.000000 metayaml-1.2/metayaml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 17:01:07.345117 metayaml-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      822 2023-06-18 17:00:08.000000 metayaml-1.2/setup.py
```

### Comparing `metayaml-1.1/PKG-INFO` & `metayaml-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metayaml
-Version: 1.1
+Version: 1.2
 Summary: Enhancements of yaml format to support include and python expression
 Home-page: https://bitbucket.org/atagunov/metayaml/
 Author: Anton Tagunov
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `metayaml-1.1/README.rst` & `metayaml-1.2/README.rst`

 * *Files identical despite different names*

### Comparing `metayaml-1.1/metayaml/exception.py` & `metayaml-1.2/metayaml/exception.py`

 * *Files identical despite different names*

### Comparing `metayaml-1.1/metayaml/jinja_eval.py` & `metayaml-1.2/metayaml/jinja_eval.py`

 * *Files identical despite different names*

### Comparing `metayaml-1.1/metayaml/metayaml.py` & `metayaml-1.2/metayaml/metayaml.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 
             simple_data, evaluated_value = self._eval_simple_data(val, global_data, new_path, eager=True)
             if simple_data:
                 dest[new_key] = evaluated_value
             else:
                 dest_value = dest.get(new_key)
                 if dest_value:
-                    self.merge_data(val, dest_value, global_data, path)
+                    dest[new_key] = self.merge_data(val, dest_value, global_data, path)
                 else:
                     new_dest = None
                     if isinstance(val, dict):  # add new dict to global data before full process
                         dest[new_key] = new_dest = {}
                     dest[new_key] = self.merge_data(val, new_dest, global_data, new_path)
         return dest
 
@@ -203,14 +203,16 @@
                 else:
                     raise MetaYamlExceptionPath(f"dict can't be merged to {type(dest)}", path, source)
             return self._merge_dict(source, dest, global_data, path)
 
         if isinstance(source, list):
             if dest is None:
                 dest = []
+            elif isinstance(dest, str):
+                dest = []
             elif not isinstance(dest, list):
                 raise MetaYamlExceptionPath(f"list can't be merged to {type(dest)}", path, source)
             dest.clear()
             dest.extend(self.eval(item, global_data, path + (key,), True)
                         for key, item in enumerate(source))
             return dest
```

### Comparing `metayaml-1.1/metayaml.egg-info/PKG-INFO` & `metayaml-1.2/metayaml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metayaml
-Version: 1.1
+Version: 1.2
 Summary: Enhancements of yaml format to support include and python expression
 Home-page: https://bitbucket.org/atagunov/metayaml/
 Author: Anton Tagunov
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `metayaml-1.1/setup.py` & `metayaml-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="metayaml",
-    version="1.1",
+    version="1.2",
     author="Anton Tagunov",
     packages=["metayaml"],
     url="https://bitbucket.org/atagunov/metayaml/",
     description="Enhancements of yaml format to support include and python expression",
     long_description=open('README.rst').read(),
     install_requires=['jinja2>=3.0', 'PyYAML'],
     test_suite="tests.test",
```

