# Comparing `tmp/shapes_recognition-2.1.3.tar.gz` & `tmp/shapes_recognition-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapes_recognition-2.1.3.tar", last modified: Sun Jun 18 06:00:25 2023, max compression
+gzip compressed data, was "shapes_recognition-2.1.4.tar", last modified: Sun Jun 18 09:38:30 2023, max compression
```

## Comparing `shapes_recognition-2.1.3.tar` & `shapes_recognition-2.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-18 06:00:25.728537 shapes_recognition-2.1.3/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-06-18 06:00:25.728225 shapes_recognition-2.1.3/PKG-INFO
--rw-r--r--   0 boriskravtsov   (501) staff       (20)      606 2023-02-16 10:59:45.000000 shapes_recognition-2.1.3/README.md
--rw-r--r--   0 boriskravtsov   (501) staff       (20)       38 2023-06-18 06:00:25.728618 shapes_recognition-2.1.3/setup.cfg
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1198 2023-06-18 05:59:14.000000 shapes_recognition-2.1.3/setup.py
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-18 06:00:25.727849 shapes_recognition-2.1.3/shapes_recognition.egg-info/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-06-18 06:00:25.000000 shapes_recognition-2.1.3/shapes_recognition.egg-info/PKG-INFO
--rw-r--r--   0 boriskravtsov   (501) staff       (20)      186 2023-06-18 06:00:25.000000 shapes_recognition-2.1.3/shapes_recognition.egg-info/SOURCES.txt
--rw-r--r--   0 boriskravtsov   (501) staff       (20)        1 2023-06-18 06:00:25.000000 shapes_recognition-2.1.3/shapes_recognition.egg-info/dependency_links.txt
--rw-r--r--   0 boriskravtsov   (501) staff       (20)       19 2023-06-18 06:00:25.000000 shapes_recognition-2.1.3/shapes_recognition.egg-info/top_level.txt
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-18 09:38:30.607041 shapes_recognition-2.1.4/
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-06-18 09:38:30.606763 shapes_recognition-2.1.4/PKG-INFO
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)      606 2023-02-16 10:59:45.000000 shapes_recognition-2.1.4/README.md
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)       38 2023-06-18 09:38:30.607115 shapes_recognition-2.1.4/setup.cfg
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     1198 2023-06-18 09:23:10.000000 shapes_recognition-2.1.4/setup.py
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-18 09:38:30.606386 shapes_recognition-2.1.4/shapes_recognition.egg-info/
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-06-18 09:38:30.000000 shapes_recognition-2.1.4/shapes_recognition.egg-info/PKG-INFO
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)      186 2023-06-18 09:38:30.000000 shapes_recognition-2.1.4/shapes_recognition.egg-info/SOURCES.txt
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)        1 2023-06-18 09:38:30.000000 shapes_recognition-2.1.4/shapes_recognition.egg-info/dependency_links.txt
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)       19 2023-06-18 09:38:30.000000 shapes_recognition-2.1.4/shapes_recognition.egg-info/top_level.txt
```

### Comparing `shapes_recognition-2.1.3/PKG-INFO` & `shapes_recognition-2.1.4/shapes_recognition.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: shapes_recognition
-Version: 2.1.3
+Name: shapes-recognition
+Version: 2.1.4
 Summary: New Shape Matching Technology
 Home-page: https://boriskravtsov.com/
 Author: Boris Kravtsov
 Author-email: boriskravtsov.contacts@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shapes_recognition-2.1.3/README.md` & `shapes_recognition-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `shapes_recognition-2.1.3/setup.py` & `shapes_recognition-2.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="shapes_recognition",
-    version="2.1.3",
+    version="2.1.4",
     description="New Shape Matching Technology",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://boriskravtsov.com/",
     author="Boris Kravtsov",
     author_email="boriskravtsov.contacts@gmail.com",
     license="MIT",
```

### Comparing `shapes_recognition-2.1.3/shapes_recognition.egg-info/PKG-INFO` & `shapes_recognition-2.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: shapes-recognition
-Version: 2.1.3
+Name: shapes_recognition
+Version: 2.1.4
 Summary: New Shape Matching Technology
 Home-page: https://boriskravtsov.com/
 Author: Boris Kravtsov
 Author-email: boriskravtsov.contacts@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

