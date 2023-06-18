# Comparing `tmp/jetkol42-1.0.0.tar.gz` & `tmp/jetkol42-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jetkol42-1.0.0.tar", last modified: Sun Jun 18 13:44:26 2023, max compression
+gzip compressed data, was "dist\jetkol42-1.0.1.tar", last modified: Sun Jun 18 13:50:56 2023, max compression
```

## Comparing `jetkol42-1.0.0.tar` & `jetkol42-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 13:44:26.000000 jetkol42-1.0.0/
--rw-rw-rw-   0        0        0        0 2023-06-04 10:55:11.000000 jetkol42-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0      388 2023-06-18 13:44:26.000000 jetkol42-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-04 10:55:23.000000 jetkol42-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 13:44:26.000000 jetkol42-1.0.0/jetkol42.egg-info/
--rw-rw-rw-   0        0        0      388 2023-06-18 13:44:26.000000 jetkol42-1.0.0/jetkol42.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-18 13:44:26.000000 jetkol42-1.0.0/jetkol42.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 13:44:26.000000 jetkol42-1.0.0/jetkol42.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-18 13:44:26.000000 jetkol42-1.0.0/jetkol42.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-18 13:44:26.000000 jetkol42-1.0.0/jetkol42.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 13:44:26.000000 jetkol42-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      617 2023-06-18 13:43:47.000000 jetkol42-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 13:44:26.000000 jetkol42-1.0.0/terver/
--rw-rw-rw-   0        0        0       19 2023-06-04 11:46:49.000000 jetkol42-1.0.0/terver/__init__.py
--rw-rw-rw-   0        0        0    18294 2023-06-18 13:43:47.000000 jetkol42-1.0.0/terver/main.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:50:56.000000 jetkol42-1.0.1/
+-rw-rw-rw-   0        0        0        0 2023-06-04 10:55:11.000000 jetkol42-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      388 2023-06-18 13:50:56.000000 jetkol42-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-04 10:55:23.000000 jetkol42-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 13:50:55.000000 jetkol42-1.0.1/jetkol42/
+-rw-rw-rw-   0        0        0       19 2023-06-04 11:46:49.000000 jetkol42-1.0.1/jetkol42/__init__.py
+-rw-rw-rw-   0        0        0    18294 2023-06-18 13:43:47.000000 jetkol42-1.0.1/jetkol42/main.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:50:55.000000 jetkol42-1.0.1/jetkol42.egg-info/
+-rw-rw-rw-   0        0        0      388 2023-06-18 13:50:55.000000 jetkol42-1.0.1/jetkol42.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-18 13:50:55.000000 jetkol42-1.0.1/jetkol42.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 13:50:55.000000 jetkol42-1.0.1/jetkol42.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-18 13:50:55.000000 jetkol42-1.0.1/jetkol42.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-18 13:50:55.000000 jetkol42-1.0.1/jetkol42.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 13:50:56.000000 jetkol42-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      617 2023-06-18 13:50:43.000000 jetkol42-1.0.1/setup.py
```

### Comparing `jetkol42-1.0.0/setup.py` & `jetkol42-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='jetkol42',
-  version='1.0.0',
+  version='1.0.1',
   author='qdzzzxc',
   author_email='nikitstp@gmail.com',
   description='xD',
   long_description=readme(),
   long_description_content_type='text/markdown',
   packages=find_packages(),
   install_requires=['pyperclip>=1.8.2'],
```

### Comparing `jetkol42-1.0.0/terver/main.py` & `jetkol42-1.0.1/jetkol42/main.py`

 * *Files identical despite different names*

