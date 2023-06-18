# Comparing `tmp/tgsdl-1.0.4.tar.gz` & `tmp/tgsdl-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgsdl-1.0.4.tar", last modified: Sat Jun 17 09:33:58 2023, max compression
+gzip compressed data, was "tgsdl-1.0.5.tar", last modified: Sun Jun 18 16:37:33 2023, max compression
```

## Comparing `tgsdl-1.0.4.tar` & `tgsdl-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:33:58.634646 tgsdl-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-17 09:33:49.000000 tgsdl-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 09:33:49.000000 tgsdl-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-17 09:33:58.634646 tgsdl-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-17 09:33:49.000000 tgsdl-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 09:33:58.634646 tgsdl-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-17 09:33:49.000000 tgsdl-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:33:58.630646 tgsdl-1.0.4/tgsdl/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-17 09:33:49.000000 tgsdl-1.0.4/tgsdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-17 09:33:49.000000 tgsdl-1.0.4/tgsdl/tgsdl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:33:58.634646 tgsdl-1.0.4/tgsdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-17 09:33:58.000000 tgsdl-1.0.4/tgsdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-17 09:33:58.000000 tgsdl-1.0.4/tgsdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 09:33:58.000000 tgsdl-1.0.4/tgsdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-17 09:33:58.000000 tgsdl-1.0.4/tgsdl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-17 09:33:58.000000 tgsdl-1.0.4/tgsdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-17 09:33:58.000000 tgsdl-1.0.4/tgsdl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:37:33.582695 tgsdl-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-18 16:37:25.000000 tgsdl-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-18 16:37:25.000000 tgsdl-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-18 16:37:33.582695 tgsdl-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-18 16:37:25.000000 tgsdl-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 16:37:33.582695 tgsdl-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-18 16:37:25.000000 tgsdl-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:37:33.582695 tgsdl-1.0.5/tgsdl/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-18 16:37:25.000000 tgsdl-1.0.5/tgsdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-18 16:37:25.000000 tgsdl-1.0.5/tgsdl/tgsdl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:37:33.582695 tgsdl-1.0.5/tgsdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-18 16:37:33.000000 tgsdl-1.0.5/tgsdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-18 16:37:33.000000 tgsdl-1.0.5/tgsdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 16:37:33.000000 tgsdl-1.0.5/tgsdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-18 16:37:33.000000 tgsdl-1.0.5/tgsdl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 16:37:33.000000 tgsdl-1.0.5/tgsdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-18 16:37:33.000000 tgsdl-1.0.5/tgsdl.egg-info/top_level.txt
```

### Comparing `tgsdl-1.0.4/LICENSE` & `tgsdl-1.0.5/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Bevlil
+Copyright (c) 2023 Bevlill
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `tgsdl-1.0.4/PKG-INFO` & `tgsdl-1.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tgsdl
-Version: 1.0.4
+Version: 1.0.5
 Summary: Telegram Sticker Pack Downloader Library
 Home-page: https://github.com/lillisfeb/TGSDL/
-Author: Bevlil
+Author: Bevlill
 Author-email: voidlillis@gmail.com
 License: MIT
 Keywords: telegram,bot,sticker,download,stickerpack
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `tgsdl-1.0.4/README.md` & `tgsdl-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tgsdl-1.0.4/setup.py` & `tgsdl-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import os
 
 current_dir = os.path.dirname(os.path.abspath(__file__))
 readme_path = os.path.join(current_dir, 'README.md')
 
 setup(
     name='tgsdl',
-    version='1.0.4',
+    version='1.0.5',
     description='Telegram Sticker Pack Downloader Library',
-    author='Bevlil',
+    author='Bevlill',
     author_email='voidlillis@gmail.com',
     url='https://github.com/lillisfeb/TGSDL/',
     long_description = open(readme_path).read(),
     long_description_content_type='text/markdown',
     keywords=['telegram', 'bot', 'sticker', 'download', 'stickerpack'],
     packages=find_packages(),
     install_requires=[
```

### Comparing `tgsdl-1.0.4/tgsdl/tgsdl.py` & `tgsdl-1.0.5/tgsdl/tgsdl.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             thread = threading.Thread(target=self.download_file, args=(file_data, folder_name))
             thread.start()
             threads.append(thread)
 
         for thread in threads:
             thread.join()
 
-        zip_filename = f"downloads/{self.pack_name}.zip"
+        zip_filename = f"Sticker/{self.pack_name}.zip"
         shutil.make_archive(folder_name, 'zip', folder_name)
 
         shutil.rmtree(folder_name)
         #print(red("Folder removed"))
         return zip_filename
 
 
@@ -100,8 +100,8 @@
         parser.print_help()
 
 
 if __name__ == "__main__":
     try:
         main()
     except:
-        pass
+        pass
```

### Comparing `tgsdl-1.0.4/tgsdl.egg-info/PKG-INFO` & `tgsdl-1.0.5/tgsdl.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tgsdl
-Version: 1.0.4
+Version: 1.0.5
 Summary: Telegram Sticker Pack Downloader Library
 Home-page: https://github.com/lillisfeb/TGSDL/
-Author: Bevlil
+Author: Bevlill
 Author-email: voidlillis@gmail.com
 License: MIT
 Keywords: telegram,bot,sticker,download,stickerpack
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

