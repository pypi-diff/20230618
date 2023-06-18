# Comparing `tmp/english-pidgin-dictionary-0.0.4.tar.gz` & `tmp/english-pidgin-dictionary-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "english-pidgin-dictionary-0.0.4.tar", last modified: Sun Jun 18 04:48:37 2023, max compression
+gzip compressed data, was "english-pidgin-dictionary-0.0.5.tar", last modified: Sun Jun 18 04:52:56 2023, max compression
```

## Comparing `english-pidgin-dictionary-0.0.4.tar` & `english-pidgin-dictionary-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 04:48:37.384083 english-pidgin-dictionary-0.0.4/
--rw-rw-rw-   0        0        0     1065 2023-06-18 04:48:12.000000 english-pidgin-dictionary-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      483 2023-06-18 04:48:37.375554 english-pidgin-dictionary-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      572 2023-06-18 04:47:58.000000 english-pidgin-dictionary-0.0.4/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-18 04:48:37.315249 english-pidgin-dictionary-0.0.4/english_pidgin_dict/
--rw-rw-rw-   0        0        0        0 2023-06-18 04:28:20.000000 english-pidgin-dictionary-0.0.4/english_pidgin_dict/__init__.py
--rw-rw-rw-   0        0        0    76618 2023-04-26 07:53:36.000000 english-pidgin-dictionary-0.0.4/english_pidgin_dict/data.json
--rw-rw-rw-   0        0        0     1481 2023-06-18 04:41:48.000000 english-pidgin-dictionary-0.0.4/english_pidgin_dict/english_pidgin_dict.py
-drwxrwxrwx   0        0        0        0 2023-06-18 04:48:37.371254 english-pidgin-dictionary-0.0.4/english_pidgin_dictionary.egg-info/
--rw-rw-rw-   0        0        0      483 2023-06-18 04:48:36.000000 english-pidgin-dictionary-0.0.4/english_pidgin_dictionary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-06-18 04:48:37.000000 english-pidgin-dictionary-0.0.4/english_pidgin_dictionary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 04:48:36.000000 english-pidgin-dictionary-0.0.4/english_pidgin_dictionary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-18 04:48:36.000000 english-pidgin-dictionary-0.0.4/english_pidgin_dictionary.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 04:48:37.385344 english-pidgin-dictionary-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      789 2023-06-18 04:43:31.000000 english-pidgin-dictionary-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 04:52:56.053084 english-pidgin-dictionary-0.0.5/
+-rw-rw-rw-   0        0        0     1065 2023-06-18 04:48:12.000000 english-pidgin-dictionary-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      525 2023-06-18 04:52:56.051090 english-pidgin-dictionary-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      572 2023-06-18 04:47:58.000000 english-pidgin-dictionary-0.0.5/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 04:52:55.994357 english-pidgin-dictionary-0.0.5/english_pidgin_dict/
+-rw-rw-rw-   0        0        0        0 2023-06-18 04:28:20.000000 english-pidgin-dictionary-0.0.5/english_pidgin_dict/__init__.py
+-rw-rw-rw-   0        0        0    76618 2023-04-26 07:53:36.000000 english-pidgin-dictionary-0.0.5/english_pidgin_dict/data.json
+-rw-rw-rw-   0        0        0     1481 2023-06-18 04:41:48.000000 english-pidgin-dictionary-0.0.5/english_pidgin_dict/english_pidgin_dict.py
+drwxrwxrwx   0        0        0        0 2023-06-18 04:52:56.043111 english-pidgin-dictionary-0.0.5/english_pidgin_dictionary.egg-info/
+-rw-rw-rw-   0        0        0      525 2023-06-18 04:52:55.000000 english-pidgin-dictionary-0.0.5/english_pidgin_dictionary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-06-18 04:52:55.000000 english-pidgin-dictionary-0.0.5/english_pidgin_dictionary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 04:52:55.000000 english-pidgin-dictionary-0.0.5/english_pidgin_dictionary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-18 04:52:55.000000 english-pidgin-dictionary-0.0.5/english_pidgin_dictionary.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 04:52:56.054082 english-pidgin-dictionary-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      831 2023-06-18 04:52:43.000000 english-pidgin-dictionary-0.0.5/setup.py
```

### Comparing `english-pidgin-dictionary-0.0.4/LICENSE.txt` & `english-pidgin-dictionary-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `english-pidgin-dictionary-0.0.4/README.txt` & `english-pidgin-dictionary-0.0.5/README.txt`

 * *Files identical despite different names*

### Comparing `english-pidgin-dictionary-0.0.4/english_pidgin_dict/data.json` & `english-pidgin-dictionary-0.0.5/english_pidgin_dict/data.json`

 * *Files identical despite different names*

### Comparing `english-pidgin-dictionary-0.0.4/english_pidgin_dict/english_pidgin_dict.py` & `english-pidgin-dictionary-0.0.5/english_pidgin_dict/english_pidgin_dict.py`

 * *Files identical despite different names*

### Comparing `english-pidgin-dictionary-0.0.4/setup.py` & `english-pidgin-dictionary-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setup(
     name='english-pidgin-dictionary',
-    version='0.0.4',
+    version='0.0.5',
     author='Isaac Yakubu',
     author_email='engrisaac1234@gmail.com',
     description='English-Pidgin Dictionary Package',
-    long_description="simple dictionary",
+    long_description="A simple pidgin-english dictionary for various applications",
     long_description_content_type='text/markdown',
     url='https://github.com/Zeecoworld/pidgin-english-dictionary',
     packages=['english_pidgin_dict'],
     include_package_data=True,
     package_data={
         'english_pidgin_dict': ['data.json'],
     },
```

