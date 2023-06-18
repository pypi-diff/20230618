# Comparing `tmp/sweatDB-2.0.5.tar.gz` & `tmp/sweatDB-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweatDB-2.0.5.tar", last modified: Sun Jun 18 05:08:32 2023, max compression
+gzip compressed data, was "sweatDB-2.0.6.tar", last modified: Sun Jun 18 12:08:16 2023, max compression
```

## Comparing `sweatDB-2.0.5.tar` & `sweatDB-2.0.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-18 05:08:32.129825 sweatDB-2.0.5/
--rw-r--r--   0 sweat     (1000) sweat     (1000)      286 2023-06-18 05:08:32.129825 sweatDB-2.0.5/PKG-INFO
--rw-r--r--   0 sweat     (1000) sweat     (1000)       81 2023-06-17 12:33:57.000000 sweatDB-2.0.5/pyproject.toml
--rw-r--r--   0 sweat     (1000) sweat     (1000)       38 2023-06-18 05:08:32.129825 sweatDB-2.0.5/setup.cfg
--rw-r--r--   0 sweat     (1000) sweat     (1000)      535 2023-06-18 05:08:15.000000 sweatDB-2.0.5/setup.py
-drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-18 05:08:32.129825 sweatDB-2.0.5/sweatDB/
--rw-r--r--   0 sweat     (1000) sweat     (1000)     3418 2023-06-18 04:53:24.000000 sweatDB-2.0.5/sweatDB/__init__.py
--rw-r--r--   0 sweat     (1000) sweat     (1000)     2249 2023-06-17 12:39:49.000000 sweatDB-2.0.5/sweatDB/sweatDB.py
-drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-18 05:08:32.129825 sweatDB-2.0.5/sweatDB.egg-info/
--rw-r--r--   0 sweat     (1000) sweat     (1000)      286 2023-06-18 05:08:32.000000 sweatDB-2.0.5/sweatDB.egg-info/PKG-INFO
--rw-r--r--   0 sweat     (1000) sweat     (1000)      186 2023-06-18 05:08:32.000000 sweatDB-2.0.5/sweatDB.egg-info/SOURCES.txt
--rw-r--r--   0 sweat     (1000) sweat     (1000)        1 2023-06-18 05:08:32.000000 sweatDB-2.0.5/sweatDB.egg-info/dependency_links.txt
--rw-r--r--   0 sweat     (1000) sweat     (1000)        8 2023-06-18 05:08:32.000000 sweatDB-2.0.5/sweatDB.egg-info/top_level.txt
+drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-18 12:08:16.521621 sweatDB-2.0.6/
+-rw-r--r--   0 sweat     (1000) sweat     (1000)      286 2023-06-18 12:08:16.521621 sweatDB-2.0.6/PKG-INFO
+-rw-r--r--   0 sweat     (1000) sweat     (1000)       81 2023-06-17 12:33:57.000000 sweatDB-2.0.6/pyproject.toml
+-rw-r--r--   0 sweat     (1000) sweat     (1000)       38 2023-06-18 12:08:16.521621 sweatDB-2.0.6/setup.cfg
+-rw-r--r--   0 sweat     (1000) sweat     (1000)      541 2023-06-18 12:00:53.000000 sweatDB-2.0.6/setup.py
+drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-18 12:08:16.517621 sweatDB-2.0.6/sweatDB/
+-rw-r--r--   0 sweat     (1000) sweat     (1000)     3891 2023-06-18 11:50:17.000000 sweatDB-2.0.6/sweatDB/__init__.py
+-rw-r--r--   0 sweat     (1000) sweat     (1000)     2249 2023-06-17 12:39:49.000000 sweatDB-2.0.6/sweatDB/sweatDB.py
+drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-18 12:08:16.521621 sweatDB-2.0.6/sweatDB.egg-info/
+-rw-r--r--   0 sweat     (1000) sweat     (1000)      286 2023-06-18 12:08:16.000000 sweatDB-2.0.6/sweatDB.egg-info/PKG-INFO
+-rw-r--r--   0 sweat     (1000) sweat     (1000)      216 2023-06-18 12:08:16.000000 sweatDB-2.0.6/sweatDB.egg-info/SOURCES.txt
+-rw-r--r--   0 sweat     (1000) sweat     (1000)        1 2023-06-18 12:08:16.000000 sweatDB-2.0.6/sweatDB.egg-info/dependency_links.txt
+-rw-r--r--   0 sweat     (1000) sweat     (1000)        5 2023-06-18 12:08:16.000000 sweatDB-2.0.6/sweatDB.egg-info/requires.txt
+-rw-r--r--   0 sweat     (1000) sweat     (1000)        8 2023-06-18 12:08:16.000000 sweatDB-2.0.6/sweatDB.egg-info/top_level.txt
```

### Comparing `sweatDB-2.0.5/setup.py` & `sweatDB-2.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 setup(
     name="sweatDB",
-    version='2.0.5',
+    version='2.0.6',
     author="0xsweat",
     author_email="<0x.sweat@tutanota.com>",
     description='A python3 DBMS',
     long_description_content_type="text/markdown",
     long_description='A database management system with an easier syntax than SQL',
     packages=find_packages(),
-    install_requires=[],
+    install_requires=['lzma'],
     keywords=['python', 'python database management system', 'DBMS'],
     classifiers=[]
 )
```

### Comparing `sweatDB-2.0.5/sweatDB/__init__.py` & `sweatDB-2.0.6/sweatDB/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,89 +1,99 @@
 import datetime
 import os
+import lzma
 version = "v2.0"
 e = os.path.isfile
-
+c = lzma.LZMACompressor()
+lf = lzma.LZMAFile
 class actions :
     
     # Create a database.
     
     def create(db):
         if e(db):
             raise Exception(f"{db} already exists")
         else:
-            open(db,'w').write(f"DATABASE NAME : {db} TIME CREATED : {datetime.datetime.utcnow()} CREATED WITH https://pypi.org/project/sweatDB/ {version}\n")
-    
+            a = bytes(f"DATABASE NAME : {db} TIME CREATED : {datetime.datetime.utcnow()} CREATED WITH https://pypi.org/project/sweatDB/ {version}\n",'utf-8')
+            lf(db,'wb').write(a)
+
     # Delete an item or database.
     
     def delete(db,item='',delete_type='item'):
         if e(db) != True:
             return f"Database : {db} doesn't exist"
         if delete_type == "db":
             os.remove(db)
         elif item == '':
             raise Exception('No item specified')
         else:
-            a = open(db, 'r').read().split("\n")
-            open(db, 'w').write("".join([f"{x}\n" for x in a if x.startswith(f'{item}') == False])[:-1])
-
+            with lf(db, 'rb') as f:
+                a = str(f.read(),'utf-8').split("\n")
+                f.close()
+            with lf(db, 'wb')as f:
+                f.write(bytes("".join([f"{x}\n" for x in a if x.startswith(f'{item}') == False])[:-1],'utf-8'))
+                f.close()
     # Add an item to a database.
 
     def add(db,name,value):
         if e(db):
-            open(db, 'a').write(f'{name} {value}\n')
+            with lf(db,'ab') as f:
+                f.write(bytes(f'{name} {value}\n','utf-8'))
+                f.close()
         else:
             raise Exception(f'Database {db} not found')
 
     # View ALL items, An item, item names, info, item count, and you can specify the limit with start && end.
 
     def view(db,option='all',item='',start=1,end=0):
         option = option.lower()
         if e(db) != True:
             raise Exception(f'Database {db} not found')
         elif option == "all":
-            c = open(db, 'r').read()
+            c = str(lf(db, 'rb').read(),'utf-8')
             if start < end and start > 0:
                 return ''.join(f'{x}\n' for x in c.split("\n")[start + 1:end + 2])
             else:
                 return c[:-1]
         elif option == "item":
-            b = open(db, 'r').read().split("\n")[1:]
+            with lf(db, 'r')as f:
+                b = str(f.read(),'utf-8').split("\n")[1:]
+                f.close()
             output = ''
             for i in b:
                 if i.startswith(f'{item}'):
                     output += ''.join([f'{x} ' for x in i.split(" ")[1:]])[:-1] + "\n"
             return output
         elif option == "items":
             if start > end and start == 1:
-                return(''.join([f'{x.split(" ")[0]}\n' for x in open(db, 'r').read().split('\n')[1:]])[:-1])
+                return(''.join([f'{x.split(" ")[0]}\n' for x in str(lf(db, 'rb').read(),'utf-8').split('\n')[1:]])[:-1])
             else:
-                return(''.join([f'{x.split(" ")[0]}\n' for x in open(db, 'r').read().split('\n')[start + 1:end + 2]])[:-1])
+                return(''.join([f'{x.split(" ")[0]}\n' for x in str(lf(db, 'rb').read(),'utf-8').split('\n')[start + 1:end + 2]])[:-1])
         elif option == "info":
-            return(open(db, 'r').read().split("\n")[0])
+            return(str(lf(db, 'rb').read(),'utf-8').split("\n")[0])
         elif option == "count":
-            return(open(db, 'r').read().count("\n") - 1)
+            return(str(lf(db, 'rb').read(),'utf-8').count("\n") - 1)
         elif option == "iv":
-            b = open(db, 'r').read().split("\n")[1:]
+            b = str(lf(db, 'rb').read(),'utf-8').split("\n")[1:]
             output = ''
             if item != '':
                 for x in b:
                     if x.startswith(f'{item}'):
                         output += f'{x}\n'
                 return output
             else:
-                return(''.join([f'{x}\n' for x in open(db, 'r').read().split('\n')[1:]])[:-1])
+                return(''.join([f'{x}\n' for x in str(lf(db, 'rb').read(),'utf-8').split('\n')[1:]])[:-1])
         else:
-            return(''.join([f'{x}\n' for x in open(db, 'r').read().split('\n')[1:]])[:-1])
+            return(''.join([f'{x}\n' for x in str(lf(db, 'rb').read(),'utf-8').split('\n')[1:]])[:-1])
                 
     # Edit an item in a database.
 
     def edit(db,item,value,t='value'):
         if e(db) != True:
             return f'Database {db} does not exist'
-        b = open(db, 'r').read().split("\n")
+        b = str(lf(db, 'rb').read(),'utf-8').split("\n")
         for x in range(len(b)):
             if b[x].startswith(f'{item}') and t=='value':
                 b[x] = f"{item} {value}"
             elif b[x].startswith(f'{item}') and t!='value':
                 b[x] = f"{value} {''.join(f'{a} ' for a in [b[x].split(' ')[1:]])[:-1]}"
-        open(db, 'w').write("".join([f"{x}\n" for x in b])[:-1])
+        lf(db, 'wb').write(bytes("".join([f"{x}\n" for x in b])[:-1],'utf-8'))
```

### Comparing `sweatDB-2.0.5/sweatDB/sweatDB.py` & `sweatDB-2.0.6/sweatDB/sweatDB.py`

 * *Files identical despite different names*

