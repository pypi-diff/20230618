# Comparing `tmp/pdf_divider-1.1.0.tar.gz` & `tmp/pdf_divider-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_divider-1.1.0.tar", last modified: Sun Jun 18 11:03:41 2023, max compression
+gzip compressed data, was "pdf_divider-1.2.0.tar", last modified: Sun Jun 18 11:14:28 2023, max compression
```

## Comparing `pdf_divider-1.1.0.tar` & `pdf_divider-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 11:03:41.272773 pdf_divider-1.1.0/
--rw-rw-rw-   0        0        0     1834 2023-06-18 09:32:09.000000 pdf_divider-1.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      419 2023-06-18 11:03:41.271563 pdf_divider-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-06-18 03:31:20.000000 pdf_divider-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 11:03:41.255248 pdf_divider-1.1.0/pdf_divider/
--rw-rw-rw-   0        0        0        0 2023-06-18 02:37:36.000000 pdf_divider-1.1.0/pdf_divider/__init__.py
--rw-rw-rw-   0        0        0     8690 2023-06-18 11:00:43.000000 pdf_divider-1.1.0/pdf_divider/pdf_divider.py
-drwxrwxrwx   0        0        0        0 2023-06-18 11:03:41.268756 pdf_divider-1.1.0/pdf_divider.egg-info/
--rw-rw-rw-   0        0        0      419 2023-06-18 11:03:41.000000 pdf_divider-1.1.0/pdf_divider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-06-18 11:03:41.000000 pdf_divider-1.1.0/pdf_divider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 11:03:41.000000 pdf_divider-1.1.0/pdf_divider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-18 11:03:41.000000 pdf_divider-1.1.0/pdf_divider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-18 11:03:41.000000 pdf_divider-1.1.0/pdf_divider.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 11:03:41.272773 pdf_divider-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      549 2023-06-18 11:03:16.000000 pdf_divider-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 11:14:28.161086 pdf_divider-1.2.0/
+-rw-rw-rw-   0        0        0     1834 2023-06-18 09:32:09.000000 pdf_divider-1.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      419 2023-06-18 11:14:28.159092 pdf_divider-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-06-18 11:14:18.000000 pdf_divider-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 11:14:28.143513 pdf_divider-1.2.0/pdf_divider/
+-rw-rw-rw-   0        0        0        0 2023-06-18 02:37:36.000000 pdf_divider-1.2.0/pdf_divider/__init__.py
+-rw-rw-rw-   0        0        0     8868 2023-06-18 11:14:06.000000 pdf_divider-1.2.0/pdf_divider/pdf_divider.py
+drwxrwxrwx   0        0        0        0 2023-06-18 11:14:28.156072 pdf_divider-1.2.0/pdf_divider.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-06-18 11:14:28.000000 pdf_divider-1.2.0/pdf_divider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-06-18 11:14:28.000000 pdf_divider-1.2.0/pdf_divider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 11:14:28.000000 pdf_divider-1.2.0/pdf_divider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-18 11:14:28.000000 pdf_divider-1.2.0/pdf_divider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-18 11:14:28.000000 pdf_divider-1.2.0/pdf_divider.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 11:14:28.161086 pdf_divider-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      549 2023-06-18 11:13:54.000000 pdf_divider-1.2.0/setup.py
```

### Comparing `pdf_divider-1.1.0/LICENSE.txt` & `pdf_divider-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pdf_divider-1.1.0/pdf_divider/pdf_divider.py` & `pdf_divider-1.2.0/pdf_divider/pdf_divider.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,34 +148,38 @@
     for b in del_over_lst_second:
         if len(b) > 512:
             oversize += 1
 
     ## 處理檔案名稱
     name_start_index = filename.rfind('/')
     filename = filename[name_start_index+1 : -4]
+    file_path = filename[0:name_start_index]
     
     ## 判斷 del_over_lst_second 中是否有東西(有沒有分段結果) 有->輸出 沒有->再處理
     if len(del_over_lst_second) == 0:
         print("lst is empty: ", filename)
-        print(f'\n{filename} is empty\n')
+        print(f'\n{filename} is empty')
         return f'\n{filename} is empty\n'
     else:
         ## output
         if oversize == 0:
             df = pd.DataFrame(del_over_lst_second)
             df.columns = ['Block']
             df.dropna(axis=0, how='any', inplace=True)
             output_filename = f'{filename}_divided.csv'
-            output_path = os.path.join(output_path, output_filename)
+            if len(output_path) == 0:
+                output_path = os.path.join(file_path, output_filename)
+            else:
+                output_path = os.path.join(output_path, output_filename)
             try:
                 df.to_csv(output_path, index=False, encoding='UTF-8-Sig')
-                print(f'{filename} finished dividing\n')
+                print(f'\n{filename} finished dividing\n')
                 return f'{filename} finished dividing\n'
             except UnicodeEncodeError:
-                print("have UnicodeEncodeError but finished dividing")
+                print("\nhave UnicodeEncodeError but finished dividing")
                 return "UnicodeEncodeError, but finished dividing"
             except Exception as e:
                 print(e)       
         else:
             print(f'package need to be modify')
             return f'{filename} oversize'
```

### Comparing `pdf_divider-1.1.0/setup.py` & `pdf_divider-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pdf_divider',
-    version='1.1.0',
+    version='1.2.0',
     author='yunsi lin',
     author_email='yunsi0115@gmail.com',
     description='divide chinese pdf file into blocks within 512',
     packages=find_packages(),
     install_requires=[
         'pymupdf',
         'fitz',
```

