# Comparing `tmp/pdf_divider-1.0.0.tar.gz` & `tmp/pdf_divider-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_divider-1.0.0.tar", last modified: Sun Jun 18 10:39:28 2023, max compression
+gzip compressed data, was "pdf_divider-1.1.0.tar", last modified: Sun Jun 18 11:03:41 2023, max compression
```

## Comparing `pdf_divider-1.0.0.tar` & `pdf_divider-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 10:39:28.962901 pdf_divider-1.0.0/
--rw-rw-rw-   0        0        0     1834 2023-06-18 09:32:09.000000 pdf_divider-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0      419 2023-06-18 10:39:28.961778 pdf_divider-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-06-18 03:31:20.000000 pdf_divider-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 10:39:28.953486 pdf_divider-1.0.0/pdf_divider/
--rw-rw-rw-   0        0        0        0 2023-06-18 02:37:36.000000 pdf_divider-1.0.0/pdf_divider/__init__.py
--rw-rw-rw-   0        0        0     8987 2023-06-18 03:25:53.000000 pdf_divider-1.0.0/pdf_divider/pdf_divider.py
-drwxrwxrwx   0        0        0        0 2023-06-18 10:39:28.960759 pdf_divider-1.0.0/pdf_divider.egg-info/
--rw-rw-rw-   0        0        0      419 2023-06-18 10:39:28.000000 pdf_divider-1.0.0/pdf_divider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-06-18 10:39:28.000000 pdf_divider-1.0.0/pdf_divider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 10:39:28.000000 pdf_divider-1.0.0/pdf_divider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-18 10:39:28.000000 pdf_divider-1.0.0/pdf_divider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-18 10:39:28.000000 pdf_divider-1.0.0/pdf_divider.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 10:39:28.962901 pdf_divider-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      549 2023-06-18 10:25:01.000000 pdf_divider-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 11:03:41.272773 pdf_divider-1.1.0/
+-rw-rw-rw-   0        0        0     1834 2023-06-18 09:32:09.000000 pdf_divider-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      419 2023-06-18 11:03:41.271563 pdf_divider-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-06-18 03:31:20.000000 pdf_divider-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 11:03:41.255248 pdf_divider-1.1.0/pdf_divider/
+-rw-rw-rw-   0        0        0        0 2023-06-18 02:37:36.000000 pdf_divider-1.1.0/pdf_divider/__init__.py
+-rw-rw-rw-   0        0        0     8690 2023-06-18 11:00:43.000000 pdf_divider-1.1.0/pdf_divider/pdf_divider.py
+drwxrwxrwx   0        0        0        0 2023-06-18 11:03:41.268756 pdf_divider-1.1.0/pdf_divider.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-06-18 11:03:41.000000 pdf_divider-1.1.0/pdf_divider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-06-18 11:03:41.000000 pdf_divider-1.1.0/pdf_divider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 11:03:41.000000 pdf_divider-1.1.0/pdf_divider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-18 11:03:41.000000 pdf_divider-1.1.0/pdf_divider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-18 11:03:41.000000 pdf_divider-1.1.0/pdf_divider.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 11:03:41.272773 pdf_divider-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      549 2023-06-18 11:03:16.000000 pdf_divider-1.1.0/setup.py
```

### Comparing `pdf_divider-1.0.0/LICENSE.txt` & `pdf_divider-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pdf_divider-1.0.0/pdf_divider/pdf_divider.py` & `pdf_divider-1.1.0/pdf_divider/pdf_divider.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,18 +161,15 @@
     else:
         ## output
         if oversize == 0:
             df = pd.DataFrame(del_over_lst_second)
             df.columns = ['Block']
             df.dropna(axis=0, how='any', inplace=True)
             output_filename = f'{filename}_divided.csv'
-            if len(output_path) == 0:
-                output_path = os.path.join(current_dir, output_filename)
-            else:
-                output_path = os.path.join(output_path, output_filename)
+            output_path = os.path.join(output_path, output_filename)
             try:
                 df.to_csv(output_path, index=False, encoding='UTF-8-Sig')
                 print(f'{filename} finished dividing\n')
                 return f'{filename} finished dividing\n'
             except UnicodeEncodeError:
                 print("have UnicodeEncodeError but finished dividing")
                 return "UnicodeEncodeError, but finished dividing"
@@ -262,10 +259,8 @@
                     list(y_gap_list).append(y)
                 else:
                     s += content
                     list(y_gap_list).append(y)
 
             # for 迴圈跑完把剩下的段落文字加到 list 中
             if len(s) != 0:
-                whole_blocks_lst.append(s)
-
-# pdf_divider('C:/Users/cherr/大學專案/pdf_divider/pdf_divider/110306079_商事法心得.pdf', remove_b_list=False, output_path='c:/Users/cherr/大學專案')
+                whole_blocks_lst.append(s)
```

### Comparing `pdf_divider-1.0.0/setup.py` & `pdf_divider-1.1.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pdf_divider',
-    version='1.0.0',
+    version='1.1.0',
     author='yunsi lin',
     author_email='yunsi0115@gmail.com',
     description='divide chinese pdf file into blocks within 512',
     packages=find_packages(),
     install_requires=[
         'pymupdf',
         'fitz',
```

