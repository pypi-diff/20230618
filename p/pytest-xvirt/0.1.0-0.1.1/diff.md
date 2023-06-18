# Comparing `tmp/pytest-xvirt-0.1.0.tar.gz` & `tmp/pytest-xvirt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/simone/Documents/python/pytest-xvirt/dist/.tmp-qywes6ha/pytest-xvirt-0.1.0.tar", last modified: Sun Jun 18 16:26:30 2023, max compression
+gzip compressed data, was "/home/simone/Documents/python/pytest-xvirt/dist/.tmp-fix0k9ry/pytest-xvirt-0.1.1.tar", last modified: Sun Jun 18 16:28:31 2023, max compression
```

## Comparing `pytest-xvirt-0.1.0.tar` & `pytest-xvirt-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-06-18 16:26:30.000000 pytest-xvirt-0.1.0/
--rw-rw-r--   0 simone    (1000) simone    (1000)     3248 2023-06-18 16:26:30.000000 pytest-xvirt-0.1.0/PKG-INFO
--rw-rw-r--   0 simone    (1000) simone    (1000)     2046 2023-04-02 16:47:36.000000 pytest-xvirt-0.1.0/README.rst
--rw-rw-r--   0 simone    (1000) simone    (1000)      236 2023-06-18 16:26:30.000000 pytest-xvirt-0.1.0/setup.cfg
--rw-rw-r--   0 simone    (1000) simone    (1000)     1708 2023-06-18 14:51:03.000000 pytest-xvirt-0.1.0/setup.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-06-18 16:26:30.000000 pytest-xvirt-0.1.0/src/
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-06-18 16:26:30.000000 pytest-xvirt-0.1.0/src/pytest_xvirt.egg-info/
--rw-rw-r--   0 simone    (1000) simone    (1000)     3248 2023-06-18 16:26:30.000000 pytest-xvirt-0.1.0/src/pytest_xvirt.egg-info/PKG-INFO
--rw-rw-r--   0 simone    (1000) simone    (1000)      550 2023-06-18 16:26:30.000000 pytest-xvirt-0.1.0/src/pytest_xvirt.egg-info/SOURCES.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-06-18 16:26:30.000000 pytest-xvirt-0.1.0/src/pytest_xvirt.egg-info/dependency_links.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)       32 2023-06-18 16:26:30.000000 pytest-xvirt-0.1.0/src/pytest_xvirt.egg-info/entry_points.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-15 17:04:00.000000 pytest-xvirt-0.1.0/src/pytest_xvirt.egg-info/not-zip-safe
--rw-rw-r--   0 simone    (1000) simone    (1000)       14 2023-06-18 16:26:30.000000 pytest-xvirt-0.1.0/src/pytest_xvirt.egg-info/requires.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)       19 2023-06-18 16:26:30.000000 pytest-xvirt-0.1.0/src/pytest_xvirt.egg-info/top_level.txt
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-06-18 16:26:30.000000 pytest-xvirt-0.1.0/src/xvirt/
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-04-15 17:01:26.000000 pytest-xvirt-0.1.0/src/xvirt/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      561 2023-05-14 17:39:36.000000 pytest-xvirt-0.1.0/src/xvirt/collectors.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-06-18 16:26:30.000000 pytest-xvirt-0.1.0/src/xvirt/empty/
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-04-15 18:10:34.000000 pytest-xvirt-0.1.0/src/xvirt/empty/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1520 2023-05-14 17:23:30.000000 pytest-xvirt-0.1.0/src/xvirt/events.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      361 2023-05-10 19:17:10.000000 pytest-xvirt-0.1.0/src/xvirt/newhooks.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     2605 2023-05-14 17:35:10.000000 pytest-xvirt-0.1.0/src/xvirt/plugin.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-06-18 16:26:30.000000 pytest-xvirt-0.1.0/tests/
--rw-rw-r--   0 simone    (1000) simone    (1000)     1485 2023-05-21 16:30:01.000000 pytest-xvirt-0.1.0/tests/test_collectors.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      873 2023-06-17 14:59:06.000000 pytest-xvirt-0.1.0/tests/test_end2end.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1571 2023-05-14 17:35:41.000000 pytest-xvirt-0.1.0/tests/test_newhook_notify.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     2414 2023-06-17 15:02:22.000000 pytest-xvirt-0.1.0/tests/test_newhook_setup.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3248 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/PKG-INFO
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2046 2023-04-02 16:47:36.000000 pytest-xvirt-0.1.1/README.rst
+-rw-rw-r--   0 simone    (1000) simone    (1000)      236 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/setup.cfg
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1708 2023-06-18 16:28:27.000000 pytest-xvirt-0.1.1/setup.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/src/
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/src/pytest_xvirt.egg-info/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3248 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/src/pytest_xvirt.egg-info/PKG-INFO
+-rw-rw-r--   0 simone    (1000) simone    (1000)      550 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/src/pytest_xvirt.egg-info/SOURCES.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/src/pytest_xvirt.egg-info/dependency_links.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)       32 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/src/pytest_xvirt.egg-info/entry_points.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-15 17:04:00.000000 pytest-xvirt-0.1.1/src/pytest_xvirt.egg-info/not-zip-safe
+-rw-rw-r--   0 simone    (1000) simone    (1000)       14 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/src/pytest_xvirt.egg-info/requires.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)       19 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/src/pytest_xvirt.egg-info/top_level.txt
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/src/xvirt/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-04-15 17:01:26.000000 pytest-xvirt-0.1.1/src/xvirt/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      561 2023-05-14 17:39:36.000000 pytest-xvirt-0.1.1/src/xvirt/collectors.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/src/xvirt/empty/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-04-15 18:10:34.000000 pytest-xvirt-0.1.1/src/xvirt/empty/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1520 2023-05-14 17:23:30.000000 pytest-xvirt-0.1.1/src/xvirt/events.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      361 2023-05-10 19:17:10.000000 pytest-xvirt-0.1.1/src/xvirt/newhooks.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2605 2023-05-14 17:35:10.000000 pytest-xvirt-0.1.1/src/xvirt/plugin.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/tests/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1485 2023-05-21 16:30:01.000000 pytest-xvirt-0.1.1/tests/test_collectors.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      873 2023-06-17 14:59:06.000000 pytest-xvirt-0.1.1/tests/test_end2end.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1571 2023-05-14 17:35:41.000000 pytest-xvirt-0.1.1/tests/test_newhook_notify.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2414 2023-06-17 15:02:22.000000 pytest-xvirt-0.1.1/tests/test_newhook_setup.py
```

### Comparing `pytest-xvirt-0.1.0/PKG-INFO` & `pytest-xvirt-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-xvirt
-Version: 0.1.0
+Version: 0.1.1
 Summary: A pytest plugin to virtualize test. For example to transparently running them on a remote box.
 Home-page: https://github.com/www-py/pytest-xvirt
 Author: Simone Giacomelli, Fabrizio Lamarca
 Author-email: simone.giacomelli@gmail.com, lamarca.fabrizio@gmail.com
 Maintainer: Simone Giacomelli
 Maintainer-email: simone.giacomelli@gmail.com
 License: Apache 2.0
```

### Comparing `pytest-xvirt-0.1.0/README.rst` & `pytest-xvirt-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-xvirt-0.1.0/setup.py` & `pytest-xvirt-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding='utf-8').read()
 
 
 setup(
     name='pytest-xvirt',
-    version='0.1.0',
+    version='0.1.1',
     author='Simone Giacomelli, Fabrizio Lamarca',
     author_email='simone.giacomelli@gmail.com, lamarca.fabrizio@gmail.com',
     maintainer='Simone Giacomelli',
     maintainer_email='simone.giacomelli@gmail.com',
     license='Apache 2.0',
     url='https://github.com/www-py/pytest-xvirt',
     description='A pytest plugin to virtualize test. For example to transparently running them on a remote box.',
```

### Comparing `pytest-xvirt-0.1.0/src/pytest_xvirt.egg-info/PKG-INFO` & `pytest-xvirt-0.1.1/src/pytest_xvirt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-xvirt
-Version: 0.1.0
+Version: 0.1.1
 Summary: A pytest plugin to virtualize test. For example to transparently running them on a remote box.
 Home-page: https://github.com/www-py/pytest-xvirt
 Author: Simone Giacomelli, Fabrizio Lamarca
 Author-email: simone.giacomelli@gmail.com, lamarca.fabrizio@gmail.com
 Maintainer: Simone Giacomelli
 Maintainer-email: simone.giacomelli@gmail.com
 License: Apache 2.0
```

### Comparing `pytest-xvirt-0.1.0/src/pytest_xvirt.egg-info/SOURCES.txt` & `pytest-xvirt-0.1.1/src/pytest_xvirt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-xvirt-0.1.0/src/xvirt/collectors.py` & `pytest-xvirt-0.1.1/src/xvirt/collectors.py`

 * *Files identical despite different names*

### Comparing `pytest-xvirt-0.1.0/src/xvirt/events.py` & `pytest-xvirt-0.1.1/src/xvirt/events.py`

 * *Files identical despite different names*

### Comparing `pytest-xvirt-0.1.0/src/xvirt/plugin.py` & `pytest-xvirt-0.1.1/src/xvirt/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-xvirt-0.1.0/tests/test_collectors.py` & `pytest-xvirt-0.1.1/tests/test_collectors.py`

 * *Files identical despite different names*

### Comparing `pytest-xvirt-0.1.0/tests/test_end2end.py` & `pytest-xvirt-0.1.1/tests/test_end2end.py`

 * *Files identical despite different names*

### Comparing `pytest-xvirt-0.1.0/tests/test_newhook_notify.py` & `pytest-xvirt-0.1.1/tests/test_newhook_notify.py`

 * *Files identical despite different names*

### Comparing `pytest-xvirt-0.1.0/tests/test_newhook_setup.py` & `pytest-xvirt-0.1.1/tests/test_newhook_setup.py`

 * *Files identical despite different names*

