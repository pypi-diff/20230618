# Comparing `tmp/english-pidgin-dictionary-0.0.5.tar.gz` & `tmp/english-pidgin-dictionary-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "english-pidgin-dictionary-0.0.5.tar", last modified: Sun Jun 18 04:52:56 2023, max compression
+gzip compressed data, was "english-pidgin-dictionary-0.0.6.tar", last modified: Sun Jun 18 05:01:49 2023, max compression
```

## Comparing `english-pidgin-dictionary-0.0.5.tar` & `english-pidgin-dictionary-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 04:52:56.053084 english-pidgin-dictionary-0.0.5/
--rw-rw-rw-   0        0        0     1065 2023-06-18 04:48:12.000000 english-pidgin-dictionary-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      525 2023-06-18 04:52:56.051090 english-pidgin-dictionary-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      572 2023-06-18 04:47:58.000000 english-pidgin-dictionary-0.0.5/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-18 04:52:55.994357 english-pidgin-dictionary-0.0.5/english_pidgin_dict/
--rw-rw-rw-   0        0        0        0 2023-06-18 04:28:20.000000 english-pidgin-dictionary-0.0.5/english_pidgin_dict/__init__.py
--rw-rw-rw-   0        0        0    76618 2023-04-26 07:53:36.000000 english-pidgin-dictionary-0.0.5/english_pidgin_dict/data.json
--rw-rw-rw-   0        0        0     1481 2023-06-18 04:41:48.000000 english-pidgin-dictionary-0.0.5/english_pidgin_dict/english_pidgin_dict.py
-drwxrwxrwx   0        0        0        0 2023-06-18 04:52:56.043111 english-pidgin-dictionary-0.0.5/english_pidgin_dictionary.egg-info/
--rw-rw-rw-   0        0        0      525 2023-06-18 04:52:55.000000 english-pidgin-dictionary-0.0.5/english_pidgin_dictionary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-06-18 04:52:55.000000 english-pidgin-dictionary-0.0.5/english_pidgin_dictionary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 04:52:55.000000 english-pidgin-dictionary-0.0.5/english_pidgin_dictionary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-18 04:52:55.000000 english-pidgin-dictionary-0.0.5/english_pidgin_dictionary.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 04:52:56.054082 english-pidgin-dictionary-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      831 2023-06-18 04:52:43.000000 english-pidgin-dictionary-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 05:01:49.459723 english-pidgin-dictionary-0.0.6/
+-rw-rw-rw-   0        0        0     1065 2023-06-18 04:48:12.000000 english-pidgin-dictionary-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     1066 2023-06-18 05:01:49.458005 english-pidgin-dictionary-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      572 2023-06-18 04:47:58.000000 english-pidgin-dictionary-0.0.6/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 05:01:49.379989 english-pidgin-dictionary-0.0.6/english_pidgin_dict/
+-rw-rw-rw-   0        0        0        0 2023-06-18 04:28:20.000000 english-pidgin-dictionary-0.0.6/english_pidgin_dict/__init__.py
+-rw-rw-rw-   0        0        0    76618 2023-04-26 07:53:36.000000 english-pidgin-dictionary-0.0.6/english_pidgin_dict/data.json
+-rw-rw-rw-   0        0        0     1481 2023-06-18 04:41:48.000000 english-pidgin-dictionary-0.0.6/english_pidgin_dict/english_pidgin_dict.py
+drwxrwxrwx   0        0        0        0 2023-06-18 05:01:49.454736 english-pidgin-dictionary-0.0.6/english_pidgin_dictionary.egg-info/
+-rw-rw-rw-   0        0        0     1066 2023-06-18 05:01:49.000000 english-pidgin-dictionary-0.0.6/english_pidgin_dictionary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-06-18 05:01:49.000000 english-pidgin-dictionary-0.0.6/english_pidgin_dictionary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 05:01:49.000000 english-pidgin-dictionary-0.0.6/english_pidgin_dictionary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-18 05:01:49.000000 english-pidgin-dictionary-0.0.6/english_pidgin_dictionary.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 05:01:49.461073 english-pidgin-dictionary-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      863 2023-06-18 05:01:41.000000 english-pidgin-dictionary-0.0.6/setup.py
```

### Comparing `english-pidgin-dictionary-0.0.5/LICENSE.txt` & `english-pidgin-dictionary-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `english-pidgin-dictionary-0.0.5/README.txt` & `english-pidgin-dictionary-0.0.6/README.txt`

 * *Files identical despite different names*

### Comparing `english-pidgin-dictionary-0.0.5/english_pidgin_dict/data.json` & `english-pidgin-dictionary-0.0.6/english_pidgin_dict/data.json`

 * *Files identical despite different names*

### Comparing `english-pidgin-dictionary-0.0.5/english_pidgin_dict/english_pidgin_dict.py` & `english-pidgin-dictionary-0.0.6/english_pidgin_dict/english_pidgin_dict.py`

 * *Files identical despite different names*

### Comparing `english-pidgin-dictionary-0.0.5/setup.py` & `english-pidgin-dictionary-0.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setup(
     name='english-pidgin-dictionary',
-    version='0.0.5',
+    version='0.0.6',
     author='Isaac Yakubu',
     author_email='engrisaac1234@gmail.com',
-    description='English-Pidgin Dictionary Package',
-    long_description="A simple pidgin-english dictionary for various applications",
+    description='A simple pidgin-english dictionary for various applications',
+    long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Zeecoworld/pidgin-english-dictionary',
     packages=['english_pidgin_dict'],
     include_package_data=True,
     package_data={
         'english_pidgin_dict': ['data.json'],
     },
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
     ],
 )
+
```

