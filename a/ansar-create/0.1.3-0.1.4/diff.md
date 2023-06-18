# Comparing `tmp/ansar-create-0.1.3.tar.gz` & `tmp/ansar-create-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar-create-0.1.3.tar", last modified: Sat Jun 17 21:18:38 2023, max compression
+gzip compressed data, was "ansar-create-0.1.4.tar", last modified: Sun Jun 18 03:24:01 2023, max compression
```

## Comparing `ansar-create-0.1.3.tar` & `ansar-create-0.1.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-17 21:18:38.601198 ansar-create-0.1.3/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1106 2023-05-15 01:49:17.000000 ansar-create-0.1.3/LICENSE
--rw-rw-r--   0 scott     (1000) scott     (1000)     1563 2023-06-17 21:18:38.601198 ansar-create-0.1.3/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      901 2023-06-17 21:18:11.000000 ansar-create-0.1.3/README.md
--rw-rw-r--   0 scott     (1000) scott     (1000)      704 2023-06-17 04:47:33.000000 ansar-create-0.1.3/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2023-06-17 21:18:38.601198 ansar-create-0.1.3/setup.cfg
--rw-rw-r--   0 scott     (1000) scott     (1000)     2067 2023-06-17 04:47:37.000000 ansar-create-0.1.3/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-17 21:18:38.597198 ansar-create-0.1.3/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-17 21:18:38.597198 ansar-create-0.1.3/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-17 21:18:38.601198 ansar-create-0.1.3/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    95138 2023-06-13 20:44:27.000000 ansar-create-0.1.3/src/ansar/command/ansar_command.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-17 21:18:38.601198 ansar-create-0.1.3/src/ansar/create/
--rw-rw-r--   0 scott     (1000) scott     (1000)     4318 2023-06-17 21:18:35.000000 ansar-create-0.1.3/src/ansar/create/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9734 2023-06-14 02:34:12.000000 ansar-create-0.1.3/src/ansar/create/args.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2822 2023-06-15 04:53:33.000000 ansar-create-0.1.3/src/ansar/create/bind.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1926 2023-05-15 01:49:17.000000 ansar-create-0.1.3/src/ansar/create/coding.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    28006 2023-06-16 21:42:07.000000 ansar-create-0.1.3/src/ansar/create/framework.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    18990 2023-06-13 01:10:23.000000 ansar-create-0.1.3/src/ansar/create/home.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6175 2023-06-15 09:49:01.000000 ansar-create-0.1.3/src/ansar/create/lifecycle.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     4160 2023-06-13 01:10:23.000000 ansar-create-0.1.3/src/ansar/create/locking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6749 2023-06-13 01:10:23.000000 ansar-create-0.1.3/src/ansar/create/log.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9671 2023-06-13 01:37:58.000000 ansar-create-0.1.3/src/ansar/create/machine.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     4887 2023-06-14 01:43:19.000000 ansar-create-0.1.3/src/ansar/create/object.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10137 2023-06-13 01:10:22.000000 ansar-create-0.1.3/src/ansar/create/pending.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    32084 2023-06-15 09:41:33.000000 ansar-create-0.1.3/src/ansar/create/point.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    37125 2023-06-16 01:44:45.000000 ansar-create-0.1.3/src/ansar/create/processing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    11124 2023-06-13 01:10:22.000000 ansar-create-0.1.3/src/ansar/create/retry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6653 2023-06-13 01:10:22.000000 ansar-create-0.1.3/src/ansar/create/rolling.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7237 2023-06-15 04:39:49.000000 ansar-create-0.1.3/src/ansar/create/root.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    12869 2023-06-13 01:10:22.000000 ansar-create-0.1.3/src/ansar/create/space.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    22448 2023-06-13 01:10:22.000000 ansar-create-0.1.3/src/ansar/create/storage.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3970 2023-06-14 22:01:39.000000 ansar-create-0.1.3/src/ansar/create/test.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     5173 2023-06-13 01:10:22.000000 ansar-create-0.1.3/src/ansar/create/timing.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-17 21:18:38.601198 ansar-create-0.1.3/src/ansar_create.egg-info/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1563 2023-06-17 21:18:38.000000 ansar-create-0.1.3/src/ansar_create.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      886 2023-06-17 21:18:38.000000 ansar-create-0.1.3/src/ansar_create.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2023-06-17 21:18:38.000000 ansar-create-0.1.3/src/ansar_create.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       59 2023-06-17 21:18:38.000000 ansar-create-0.1.3/src/ansar_create.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       21 2023-06-17 21:18:38.000000 ansar-create-0.1.3/src/ansar_create.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2023-06-17 21:18:38.000000 ansar-create-0.1.3/src/ansar_create.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-18 03:24:01.795069 ansar-create-0.1.4/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-18 03:22:18.000000 ansar-create-0.1.4/LICENSE
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1569 2023-06-18 03:24:01.795069 ansar-create-0.1.4/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      901 2023-06-17 21:18:11.000000 ansar-create-0.1.4/README.md
+-rw-rw-r--   0 scott     (1000) scott     (1000)      710 2023-06-18 03:18:32.000000 ansar-create-0.1.4/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2023-06-18 03:24:01.795069 ansar-create-0.1.4/setup.cfg
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2079 2023-06-18 03:18:33.000000 ansar-create-0.1.4/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-18 03:24:01.795069 ansar-create-0.1.4/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-18 03:24:01.795069 ansar-create-0.1.4/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-18 03:24:01.795069 ansar-create-0.1.4/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    95144 2023-06-18 03:18:34.000000 ansar-create-0.1.4/src/ansar/command/ansar_command.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-18 03:24:01.795069 ansar-create-0.1.4/src/ansar/create/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     4336 2023-06-18 03:23:58.000000 ansar-create-0.1.4/src/ansar/create/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9752 2023-06-18 03:22:20.000000 ansar-create-0.1.4/src/ansar/create/args.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2828 2023-06-18 03:21:08.000000 ansar-create-0.1.4/src/ansar/create/bind.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1944 2023-06-18 03:22:20.000000 ansar-create-0.1.4/src/ansar/create/coding.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    28024 2023-06-18 03:22:21.000000 ansar-create-0.1.4/src/ansar/create/framework.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    19008 2023-06-18 03:22:21.000000 ansar-create-0.1.4/src/ansar/create/home.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6175 2023-06-15 09:49:01.000000 ansar-create-0.1.4/src/ansar/create/lifecycle.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     4178 2023-06-18 03:22:22.000000 ansar-create-0.1.4/src/ansar/create/locking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6755 2023-06-18 03:21:11.000000 ansar-create-0.1.4/src/ansar/create/log.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9677 2023-06-18 03:21:11.000000 ansar-create-0.1.4/src/ansar/create/machine.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     4905 2023-06-18 03:22:22.000000 ansar-create-0.1.4/src/ansar/create/object.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10143 2023-06-18 03:21:12.000000 ansar-create-0.1.4/src/ansar/create/pending.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    32090 2023-06-18 03:18:41.000000 ansar-create-0.1.4/src/ansar/create/point.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    37131 2023-06-18 03:21:12.000000 ansar-create-0.1.4/src/ansar/create/processing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    11142 2023-06-18 03:22:23.000000 ansar-create-0.1.4/src/ansar/create/retry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6659 2023-06-18 03:21:13.000000 ansar-create-0.1.4/src/ansar/create/rolling.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7255 2023-06-18 03:22:23.000000 ansar-create-0.1.4/src/ansar/create/root.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    12875 2023-06-18 03:21:14.000000 ansar-create-0.1.4/src/ansar/create/space.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    22466 2023-06-18 03:22:24.000000 ansar-create-0.1.4/src/ansar/create/storage.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3976 2023-06-18 03:21:15.000000 ansar-create-0.1.4/src/ansar/create/test.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     5179 2023-06-18 03:21:15.000000 ansar-create-0.1.4/src/ansar/create/timing.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-18 03:24:01.795069 ansar-create-0.1.4/src/ansar_create.egg-info/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1569 2023-06-18 03:24:01.000000 ansar-create-0.1.4/src/ansar_create.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      886 2023-06-18 03:24:01.000000 ansar-create-0.1.4/src/ansar_create.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2023-06-18 03:24:01.000000 ansar-create-0.1.4/src/ansar_create.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       59 2023-06-18 03:24:01.000000 ansar-create-0.1.4/src/ansar_create.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       21 2023-06-18 03:24:01.000000 ansar-create-0.1.4/src/ansar_create.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2023-06-18 03:24:01.000000 ansar-create-0.1.4/src/ansar_create.egg-info/top_level.txt
```

### Comparing `ansar-create-0.1.3/LICENSE` & `ansar-create-0.1.4/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-Author: Scott Woods <scott.suzuki@gmail.com>
+Author: Scott Woods <scott.18.ansar@gmail.com.com>
 MIT License
 
-Copyright (c) 2017-2022
+Copyright (c) 2017-2023 Scott Woods
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ansar-create-0.1.3/PKG-INFO` & `ansar-create-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ansar-create
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
-Author-email: Scott Woods <scott.suzuki@gmail.com>
+Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-create-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `ansar-create-0.1.3/README.md` & `ansar-create-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.3/pyproject.toml` & `ansar-create-0.1.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ansar-create"
 readme = "README.md"
 authors = [
-  { name="Scott Woods", email="scott.suzuki@gmail.com" }
+  { name="Scott Woods", email="scott.18.ansar@gmail.com.com" }
 ]
 requires-python = ">=3.7"
 classifiers=[
 	"Development Status :: 4 - Beta",
 	"Intended Audience :: Developers",
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `ansar-create-0.1.3/setup.py` & `ansar-create-0.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Standard PyPi packaging.
 # Build materials and push to pypi.org.
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 import sys
 import setuptools
 import re
 
 #
 #
 VERSION_PATTERN = re.compile(r'([0-9]+)\.([0-9]+)\.([0-9]+)')
@@ -42,15 +42,15 @@
     "ansar-encode>=0.1.78",
 ]
 
 setuptools.setup(
     name=PACKAGE,
     version=VERSION,
     author="Scott Woods",
-    author_email="scott.suzuki@gmail.com",
+    author_email="scott.18.ansar@gmail.com.com",
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     #project_urls={
     #    "Documentation": DOC_LINK,
     #},
     #classifiers=[
```

### Comparing `ansar-create-0.1.3/src/ansar/command/ansar_command.py` & `ansar-create-0.1.4/src/ansar/command/ansar_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
 # Copyright (c) 2022 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
```

### Comparing `ansar-create-0.1.3/src/ansar/create/__init__.py` & `ansar-create-0.1.4/src/ansar/create/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-create.git
 Branch: main
-Commit: 4f5daf2ac1aa5ee8c68e91cdccbae87c192d8ecc
-Version: 0.1.2 (2023-06-18@09:18:35+NZST)
+Commit: 9b8e14daabe1f054d72f6b46884d4c8114e386a2
+Version: 0.1.3 (2023-06-18@15:23:58+NZST)
 """
 
 from ansar.encode import *
 
 from .coding import Gas, breakpath
 from .space import NO_SUCH_ADDRESS
 from .space import create_an_object, find_object, destroy_an_object
```

### Comparing `ansar-create-0.1.3/src/ansar/create/args.py` & `ansar-create-0.1.4/src/ansar/create/args.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-create-0.1.3/src/ansar/create/bind.py` & `ansar-create-0.1.4/src/ansar/create/bind.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022 Scott Woods
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-create-0.1.3/src/ansar/create/coding.py` & `ansar-create-0.1.4/src/ansar/create/coding.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-create-0.1.3/src/ansar/create/framework.py` & `ansar-create-0.1.4/src/ansar/create/framework.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-create-0.1.3/src/ansar/create/home.py` & `ansar-create-0.1.4/src/ansar/create/home.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-create-0.1.3/src/ansar/create/lifecycle.py` & `ansar-create-0.1.4/src/ansar/create/lifecycle.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.3/src/ansar/create/locking.py` & `ansar-create-0.1.4/src/ansar/create/locking.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-create-0.1.3/src/ansar/create/log.py` & `ansar-create-0.1.4/src/ansar/create/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022 Scott Woods
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-create-0.1.3/src/ansar/create/machine.py` & `ansar-create-0.1.4/src/ansar/create/machine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022 Scott Woods
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-create-0.1.3/src/ansar/create/object.py` & `ansar-create-0.1.4/src/ansar/create/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-create-0.1.3/src/ansar/create/pending.py` & `ansar-create-0.1.4/src/ansar/create/pending.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022 Scott Woods
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-create-0.1.3/src/ansar/create/point.py` & `ansar-create-0.1.4/src/ansar/create/point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
 # Copyright (c) 2017 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
```

### Comparing `ansar-create-0.1.3/src/ansar/create/processing.py` & `ansar-create-0.1.4/src/ansar/create/processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022 Scott Woods
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-create-0.1.3/src/ansar/create/retry.py` & `ansar-create-0.1.4/src/ansar/create/retry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-create-0.1.3/src/ansar/create/rolling.py` & `ansar-create-0.1.4/src/ansar/create/rolling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022 Scott Woods
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-create-0.1.3/src/ansar/create/root.py` & `ansar-create-0.1.4/src/ansar/create/root.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-create-0.1.3/src/ansar/create/space.py` & `ansar-create-0.1.4/src/ansar/create/space.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022 Scott Woods
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-create-0.1.3/src/ansar/create/storage.py` & `ansar-create-0.1.4/src/ansar/create/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-create-0.1.3/src/ansar/create/test.py` & `ansar-create-0.1.4/src/ansar/create/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022 Scott Woods
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-create-0.1.3/src/ansar/create/timing.py` & `ansar-create-0.1.4/src/ansar/create/timing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022 Scott Woods
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-create-0.1.3/src/ansar_create.egg-info/PKG-INFO` & `ansar-create-0.1.4/src/ansar_create.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ansar-create
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
-Author-email: Scott Woods <scott.suzuki@gmail.com>
+Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-create-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `ansar-create-0.1.3/src/ansar_create.egg-info/SOURCES.txt` & `ansar-create-0.1.4/src/ansar_create.egg-info/SOURCES.txt`

 * *Files identical despite different names*

