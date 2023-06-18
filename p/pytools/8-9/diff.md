# Comparing `tmp/pytools-8.tar.gz` & `tmp/pytools-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytools-8.tar", last modified: Wed Apr  8 02:55:03 2009, max compression, from Unix
+gzip compressed data, was "pytools-9.tar", last modified: Wed Apr  8 14:17:59 2009, max compression, from Unix
```

## Comparing `pytools-8.tar` & `pytools-9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2009-04-08 02:55:02.000000 pytools-8/
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2009-04-08 02:55:02.000000 pytools-8/bin/
--rwxr-xr-x   0 andreas   (1000) andreas   (1000)     8010 2008-12-10 04:32:56.000000 pytools-8/bin/logtool
--rw-r--r--   0 andreas   (1000) andreas   (1000)     1126 2008-11-19 20:26:22.000000 pytools-8/bin/runalyzer
--rw-r--r--   0 andreas   (1000) andreas   (1000)     8170 2008-04-27 04:13:36.000000 pytools-8/bin/runalyzer-gather
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2009-04-08 02:55:02.000000 pytools-8/pytools.egg-info/
--rw-r--r--   0 andreas   (1000) andreas   (1000)     1603 2009-04-08 02:54:59.000000 pytools-8/pytools.egg-info/PKG-INFO
--rw-r--r--   0 andreas   (1000) andreas   (1000)      483 2009-04-08 02:55:02.000000 pytools-8/pytools.egg-info/SOURCES.txt
--rw-r--r--   0 andreas   (1000) andreas   (1000)        1 2009-04-08 02:54:59.000000 pytools-8/pytools.egg-info/dependency_links.txt
--rw-r--r--   0 andreas   (1000) root         (0)        1 2008-08-22 14:02:59.000000 pytools-8/pytools.egg-info/not-zip-safe
--rw-r--r--   0 andreas   (1000) andreas   (1000)        8 2009-04-08 02:54:59.000000 pytools-8/pytools.egg-info/top_level.txt
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2009-04-08 02:55:02.000000 pytools-8/src/
--rw-r--r--   0 andreas   (1000) andreas   (1000)    30247 2009-02-11 16:32:32.000000 pytools-8/src/__init__.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    15392 2008-04-03 18:13:30.000000 pytools-8/src/arithmetic_container.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     3804 2008-07-09 16:24:18.000000 pytools-8/src/batchjob.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     8676 2008-04-26 18:59:10.000000 pytools-8/src/datatable.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     5905 2007-09-20 15:36:41.000000 pytools-8/src/decorator.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     4532 2008-10-24 17:42:58.000000 pytools-8/src/diskdict.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     5762 2007-02-13 00:03:48.000000 pytools-8/src/grid.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     3973 2007-02-13 00:03:48.000000 pytools-8/src/lex.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    31557 2009-03-26 18:49:19.000000 pytools-8/src/log.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     3226 2009-03-20 00:33:29.000000 pytools-8/src/prefork.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     2570 2009-01-22 17:48:12.000000 pytools-8/src/refdebug.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    10408 2008-12-09 02:01:52.000000 pytools-8/src/runalyzer.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     1811 2007-11-15 06:45:27.000000 pytools-8/src/stopwatch.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2009-04-08 02:55:02.000000 pytools-8/test/
--rw-r--r--   0 andreas   (1000) andreas   (1000)      200 2009-03-20 00:33:29.000000 pytools-8/test/test-prefork.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     3589 2008-06-21 21:35:37.000000 pytools-8/test/test.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)       20 2008-04-21 18:53:56.000000 pytools-8/MANIFEST.in
--rw-r--r--   0 andreas   (1000) andreas   (1000)      169 2007-05-28 03:38:49.000000 pytools-8/README
--rw-r--r--   0 andreas   (1000) andreas   (1000)     9419 2008-04-21 18:16:42.000000 pytools-8/ez_setup.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     1918 2009-03-20 00:33:29.000000 pytools-8/setup.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     1603 2009-04-08 02:55:02.000000 pytools-8/PKG-INFO
--rw-r--r--   0 andreas   (1000) andreas   (1000)       59 2009-04-08 02:55:02.000000 pytools-8/setup.cfg
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2009-04-08 14:17:59.000000 pytools-9/
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2009-04-08 14:17:59.000000 pytools-9/bin/
+-rwxr-xr-x   0 andreas   (1000) andreas   (1000)     8010 2008-12-10 04:32:56.000000 pytools-9/bin/logtool
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     1126 2008-11-19 20:26:22.000000 pytools-9/bin/runalyzer
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     8170 2008-04-27 04:13:36.000000 pytools-9/bin/runalyzer-gather
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2009-04-08 14:17:59.000000 pytools-9/pytools.egg-info/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     1603 2009-04-08 14:17:58.000000 pytools-9/pytools.egg-info/PKG-INFO
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      483 2009-04-08 14:17:59.000000 pytools-9/pytools.egg-info/SOURCES.txt
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        1 2009-04-08 14:17:58.000000 pytools-9/pytools.egg-info/dependency_links.txt
+-rw-r--r--   0 andreas   (1000) root         (0)        1 2008-08-22 14:02:59.000000 pytools-9/pytools.egg-info/not-zip-safe
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        8 2009-04-08 14:17:58.000000 pytools-9/pytools.egg-info/top_level.txt
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2009-04-08 14:17:59.000000 pytools-9/src/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    30247 2009-02-11 16:32:32.000000 pytools-9/src/__init__.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    15392 2008-04-03 18:13:30.000000 pytools-9/src/arithmetic_container.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     3804 2008-07-09 16:24:18.000000 pytools-9/src/batchjob.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     8676 2008-04-26 18:59:10.000000 pytools-9/src/datatable.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     5905 2007-09-20 15:36:41.000000 pytools-9/src/decorator.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     4532 2008-10-24 17:42:58.000000 pytools-9/src/diskdict.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     5762 2007-02-13 00:03:48.000000 pytools-9/src/grid.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     3973 2007-02-13 00:03:48.000000 pytools-9/src/lex.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    31557 2009-03-26 18:49:19.000000 pytools-9/src/log.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     3226 2009-03-20 00:33:29.000000 pytools-9/src/prefork.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     2570 2009-01-22 17:48:12.000000 pytools-9/src/refdebug.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    10408 2008-12-09 02:01:52.000000 pytools-9/src/runalyzer.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     1811 2007-11-15 06:45:27.000000 pytools-9/src/stopwatch.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2009-04-08 14:17:59.000000 pytools-9/test/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      200 2009-03-20 00:33:29.000000 pytools-9/test/test-prefork.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     3589 2008-06-21 21:35:37.000000 pytools-9/test/test.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)       20 2008-04-21 18:53:56.000000 pytools-9/MANIFEST.in
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      169 2007-05-28 03:38:49.000000 pytools-9/README
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     9716 2008-10-02 19:50:55.000000 pytools-9/ez_setup.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     1918 2009-04-08 14:16:46.000000 pytools-9/setup.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     1603 2009-04-08 14:17:59.000000 pytools-9/PKG-INFO
+-rw-r--r--   0 andreas   (1000) andreas   (1000)       59 2009-04-08 14:17:59.000000 pytools-9/setup.cfg
```

### Comparing `pytools-8/bin/logtool` & `pytools-9/bin/logtool`

 * *Files identical despite different names*

### Comparing `pytools-8/bin/runalyzer` & `pytools-9/bin/runalyzer`

 * *Files identical despite different names*

### Comparing `pytools-8/bin/runalyzer-gather` & `pytools-9/bin/runalyzer-gather`

 * *Files identical despite different names*

### Comparing `pytools-8/pytools.egg-info/PKG-INFO` & `pytools-9/pytools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: pytools
-Version: 8
+Version: 9
 Summary: A collection of tools for Python
 Home-page: http://pypi.python.org/pypi/pytools
 Author: Andreas Kloeckner
 Author-email: inform@tiker.net
 License: MIT
 Description: 
         Pytools is a big bag of things that are "missing" from the Python standard
```

### Comparing `pytools-8/src/__init__.py` & `pytools-9/src/__init__.py`

 * *Files identical despite different names*

### Comparing `pytools-8/src/arithmetic_container.py` & `pytools-9/src/arithmetic_container.py`

 * *Files identical despite different names*

### Comparing `pytools-8/src/batchjob.py` & `pytools-9/src/batchjob.py`

 * *Files identical despite different names*

### Comparing `pytools-8/src/datatable.py` & `pytools-9/src/datatable.py`

 * *Files identical despite different names*

### Comparing `pytools-8/src/decorator.py` & `pytools-9/src/decorator.py`

 * *Files identical despite different names*

### Comparing `pytools-8/src/diskdict.py` & `pytools-9/src/diskdict.py`

 * *Files identical despite different names*

### Comparing `pytools-8/src/grid.py` & `pytools-9/src/grid.py`

 * *Files identical despite different names*

### Comparing `pytools-8/src/lex.py` & `pytools-9/src/lex.py`

 * *Files identical despite different names*

### Comparing `pytools-8/src/log.py` & `pytools-9/src/log.py`

 * *Files identical despite different names*

### Comparing `pytools-8/src/prefork.py` & `pytools-9/src/prefork.py`

 * *Files identical despite different names*

### Comparing `pytools-8/src/refdebug.py` & `pytools-9/src/refdebug.py`

 * *Files identical despite different names*

### Comparing `pytools-8/src/runalyzer.py` & `pytools-9/src/runalyzer.py`

 * *Files identical despite different names*

### Comparing `pytools-8/src/stopwatch.py` & `pytools-9/src/stopwatch.py`

 * *Files identical despite different names*

### Comparing `pytools-8/test/test.py` & `pytools-9/test/test.py`

 * *Files identical despite different names*

### Comparing `pytools-8/ez_setup.py` & `pytools-9/ez_setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 If you want to require a specific version of setuptools, set a download
 mirror, or use an alternate download directory, you can do so by supplying
 the appropriate options to ``use_setuptools()``.
 
 This file can also be run as a script to install or upgrade setuptools.
 """
 import sys
-DEFAULT_VERSION = "0.6c8"
+DEFAULT_VERSION = "0.6c9"
 DEFAULT_URL     = "http://pypi.python.org/packages/%s/s/setuptools/" % sys.version[:3]
 
 md5_data = {
     'setuptools-0.6b1-py2.3.egg': '8822caf901250d848b996b7f25c6e6ca',
     'setuptools-0.6b1-py2.4.egg': 'b79a8a403e4502fbb85ee3f1941735cb',
     'setuptools-0.6b2-py2.3.egg': '5657759d8a6d8fc44070a9d07272d99b',
     'setuptools-0.6b2-py2.4.egg': '4996a8d169d2be661fa32a6e52e4f82a',
@@ -44,31 +44,35 @@
     'setuptools-0.6c6-py2.5.egg': 'b2f8a7520709a5b34f80946de5f02f53',
     'setuptools-0.6c7-py2.3.egg': '209fdf9adc3a615e5115b725658e13e2',
     'setuptools-0.6c7-py2.4.egg': '5a8f954807d46a0fb67cf1f26c55a82e',
     'setuptools-0.6c7-py2.5.egg': '45d2ad28f9750e7434111fde831e8372',
     'setuptools-0.6c8-py2.3.egg': '50759d29b349db8cfd807ba8303f1902',
     'setuptools-0.6c8-py2.4.egg': 'cba38d74f7d483c06e9daa6070cce6de',
     'setuptools-0.6c8-py2.5.egg': '1721747ee329dc150590a58b3e1ac95b',
+    'setuptools-0.6c9-py2.3.egg': 'a83c4020414807b496e4cfbe08507c03',
+    'setuptools-0.6c9-py2.4.egg': '260a2be2e5388d66bdaee06abec6342a',
+    'setuptools-0.6c9-py2.5.egg': 'fe67c3e5a17b12c0e7c541b7ea43a8e6',
+    'setuptools-0.6c9-py2.6.egg': 'ca37b1ff16fa2ede6e19383e7b59245a',
 }
 
 import sys, os
+try: from hashlib import md5
+except ImportError: from md5 import md5
 
 def _validate_md5(egg_name, data):
     if egg_name in md5_data:
-        from md5 import md5
         digest = md5(data).hexdigest()
         if digest != md5_data[egg_name]:
             print >>sys.stderr, (
                 "md5 validation of %s failed!  (Possible download problem?)"
                 % egg_name
             )
             sys.exit(2)
     return data
 
-
 def use_setuptools(
     version=DEFAULT_VERSION, download_base=DEFAULT_URL, to_dir=os.curdir,
     download_delay=15
 ):
     """Automatically find/download setuptools and make it available on sys.path
 
     `version` should be a valid setuptools version number that is available
@@ -229,15 +233,14 @@
             print "Setuptools version",version,"or greater has been installed."
             print '(Run "ez_setup.py -U setuptools" to reinstall or upgrade.)'
 
 def update_md5(filenames):
     """Update our built-in md5 registry"""
 
     import re
-    from md5 import md5
 
     for name in filenames:
         base = os.path.basename(name)
         f = open(name,'rb')
         md5_data[base] = md5(f.read()).hexdigest()
         f.close()
 
@@ -266,7 +269,8 @@
     else:
         main(sys.argv[1:])
 
 
 
 
 
+
```

### Comparing `pytools-8/setup.py` & `pytools-9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import ez_setup
 
 ez_setup.use_setuptools()
 
 from setuptools import setup
 
 setup(name="pytools",
-      version="8",
+      version="9",
       description="A collection of tools for Python",
       long_description="""
       Pytools is a big bag of things that are "missing" from the Python standard
       library. This is mainly a dependency of my other software packages, and is
       probably of little interest to you unless you use those. If you're curious
       nonetheless, here's what's on offer:
```

### Comparing `pytools-8/PKG-INFO` & `pytools-9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: pytools
-Version: 8
+Version: 9
 Summary: A collection of tools for Python
 Home-page: http://pypi.python.org/pypi/pytools
 Author: Andreas Kloeckner
 Author-email: inform@tiker.net
 License: MIT
 Description: 
         Pytools is a big bag of things that are "missing" from the Python standard
```

