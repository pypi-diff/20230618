# Comparing `tmp/sweatDB-2.0.3.tar.gz` & `tmp/sweatDB-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweatDB-2.0.3.tar", last modified: Sun Jun 18 01:01:41 2023, max compression
+gzip compressed data, was "sweatDB-2.0.4.tar", last modified: Sun Jun 18 01:38:26 2023, max compression
```

## Comparing `sweatDB-2.0.3.tar` & `sweatDB-2.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-18 01:01:41.585434 sweatDB-2.0.3/
--rw-r--r--   0 sweat     (1000) sweat     (1000)      286 2023-06-18 01:01:41.585434 sweatDB-2.0.3/PKG-INFO
--rw-r--r--   0 sweat     (1000) sweat     (1000)       81 2023-06-17 12:33:57.000000 sweatDB-2.0.3/pyproject.toml
--rw-r--r--   0 sweat     (1000) sweat     (1000)       38 2023-06-18 01:01:41.585434 sweatDB-2.0.3/setup.cfg
--rw-r--r--   0 sweat     (1000) sweat     (1000)      535 2023-06-18 00:20:39.000000 sweatDB-2.0.3/setup.py
-drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-18 01:01:41.585434 sweatDB-2.0.3/sweatDB/
--rw-r--r--   0 sweat     (1000) sweat     (1000)     2798 2023-06-18 01:00:25.000000 sweatDB-2.0.3/sweatDB/__init__.py
--rw-r--r--   0 sweat     (1000) sweat     (1000)     2249 2023-06-17 12:39:49.000000 sweatDB-2.0.3/sweatDB/sweatDB.py
-drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-18 01:01:41.585434 sweatDB-2.0.3/sweatDB.egg-info/
--rw-r--r--   0 sweat     (1000) sweat     (1000)      286 2023-06-18 01:01:41.000000 sweatDB-2.0.3/sweatDB.egg-info/PKG-INFO
--rw-r--r--   0 sweat     (1000) sweat     (1000)      186 2023-06-18 01:01:41.000000 sweatDB-2.0.3/sweatDB.egg-info/SOURCES.txt
--rw-r--r--   0 sweat     (1000) sweat     (1000)        1 2023-06-18 01:01:41.000000 sweatDB-2.0.3/sweatDB.egg-info/dependency_links.txt
--rw-r--r--   0 sweat     (1000) sweat     (1000)        8 2023-06-18 01:01:41.000000 sweatDB-2.0.3/sweatDB.egg-info/top_level.txt
+drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-18 01:38:26.709492 sweatDB-2.0.4/
+-rw-r--r--   0 sweat     (1000) sweat     (1000)      286 2023-06-18 01:38:26.709492 sweatDB-2.0.4/PKG-INFO
+-rw-r--r--   0 sweat     (1000) sweat     (1000)       81 2023-06-17 12:33:57.000000 sweatDB-2.0.4/pyproject.toml
+-rw-r--r--   0 sweat     (1000) sweat     (1000)       38 2023-06-18 01:38:26.709492 sweatDB-2.0.4/setup.cfg
+-rw-r--r--   0 sweat     (1000) sweat     (1000)      535 2023-06-18 01:38:14.000000 sweatDB-2.0.4/setup.py
+drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-18 01:38:26.709492 sweatDB-2.0.4/sweatDB/
+-rw-r--r--   0 sweat     (1000) sweat     (1000)     2968 2023-06-18 01:28:18.000000 sweatDB-2.0.4/sweatDB/__init__.py
+-rw-r--r--   0 sweat     (1000) sweat     (1000)     2249 2023-06-17 12:39:49.000000 sweatDB-2.0.4/sweatDB/sweatDB.py
+drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-18 01:38:26.709492 sweatDB-2.0.4/sweatDB.egg-info/
+-rw-r--r--   0 sweat     (1000) sweat     (1000)      286 2023-06-18 01:38:26.000000 sweatDB-2.0.4/sweatDB.egg-info/PKG-INFO
+-rw-r--r--   0 sweat     (1000) sweat     (1000)      186 2023-06-18 01:38:26.000000 sweatDB-2.0.4/sweatDB.egg-info/SOURCES.txt
+-rw-r--r--   0 sweat     (1000) sweat     (1000)        1 2023-06-18 01:38:26.000000 sweatDB-2.0.4/sweatDB.egg-info/dependency_links.txt
+-rw-r--r--   0 sweat     (1000) sweat     (1000)        8 2023-06-18 01:38:26.000000 sweatDB-2.0.4/sweatDB.egg-info/top_level.txt
```

### Comparing `sweatDB-2.0.3/setup.py` & `sweatDB-2.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 setup(
     name="sweatDB",
-    version='2.0.3',
+    version='2.0.4',
     author="0xsweat",
     author_email="<0x.sweat@tutanota.com>",
     description='A python3 DBMS',
     long_description_content_type="text/markdown",
     long_description='A database management system with an easier syntax than SQL',
     packages=find_packages(),
     install_requires=[],
```

### Comparing `sweatDB-2.0.3/sweatDB/__init__.py` & `sweatDB-2.0.4/sweatDB/sweatDB.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,73 +1,56 @@
 import datetime
 import os
-version = "v2.0"
-e = os.path.isfile
-
 class actions :
-    
-    # Create a database.
+    version = "v2.1"
+    e = os.path.isfile
     
     def create(db):
         if e(db):
-            raise Exception(f"{db} already exists")
+            raise Exception("{db} already exists")
         else:
-            open(db,'w').write(f"DATABASE NAME : {db} TIME CREATED : {datetime.datetime.utcnow()} CREATED WITH https://pypi.org/project/sweatDB/ {version}\n")
-    
-    # Delete an item or database.
-    
-    def delete(db,delete_type,item=''):
-        if e(db) != True:
-            return f"Database : {db} doesn't exist"
-        if delete_type == "db":
+            open(db).write(f"DATABASE NAME : {db} TIME CREATED : {datetime.datetime.utcnow()} CREATED WITH https://github.com/0xsweat/sweatDB {version}\n")
+            
+    def delete(ttd,db,item=''):
+        if e(name) != True:
+            return f"Database : {name} doesn't exist"
+        if ttd == "db":
             os.remove(db)
         elif item == '':
             raise Exception('No item specified')
             a = open(db, 'r').read().split("\n")
             open(db, 'w').write("".join([f"{x}\n" for x in a if x.startswith(f'{item} ') == False])[:-1])
 
-    # Add an item to a database.
-
     def add(db,name,value):
         if e(db):
             open(db, 'a').write(f'{name} {value}\n')
         else:
             raise Exception(f'Database {db} not found')
 
-    # View ALL items, An item, item names, info, item count, and you can specify the limit with start && end.
-
     def view(db,option='all',item='',start=1,end=0):
-        option = option.lower()
         if e(db) != True:
             raise Exception(f'Database {db} not found')
         elif option == "all":
             c = open(db, 'r').read()
             if start < end and start > 0:
-                return ''.join(f'{x}\n' for x in c.split("\n")[start + 1:end + 2])
+                return ''.join(f'{x}\n' for x in c.split("\n")[start:end])
             else:
                 return c
         elif option == "item":
             b = open(db, 'r').read().split("\n")
-            output = ''
             for i in range(1,len(b)):
-                if b[i].startswith(f'{item}'):
-                    output += ''.join([f'{x} ' for x in b[i].split(" ")[1:]])[:-1] + "\n"
-            return output
+                if b[i].startswith(f'{item} '):
+                    return(''.join([f'{x} ' for x in b[i].split(" ")[1:]])[:-1])
             raise Exception(f'{item} not present in {db}')
         elif option == "items":
-            if start > end and start == 1:
-                return(''.join([f'{x.split(" ")[0]}\n' for x in open(db, 'r').read().split('\n')[1:]])[:-1])
-            else:
-                return(''.join([f'{x.split(" ")[0]}\n' for x in open(db, 'r').read().split('\n')[start + 1:end + 2]])[:-1])
+            return(''.join([f'{x.split(" ")[0]}\n' for x in open(db, 'r').read().split('\n')[1:]])[:-2])
         elif option == "info":
             return(open(db, 'r').read().split("\n")[0])
-        elif option == "count":
+        elif option == "itemcount":
             return(open(db, 'r').read().count("\n") - 1)
-                
-    # Edit an item in a database.
 
     def edit(db,item,value):
         if e(db) != True:
             return f'Database {db} does not exist'
         b = open(db, 'r').read().split("\n")
         for x in range(len(b)):
             if b[x].startswith(f'{item} '):
```

### Comparing `sweatDB-2.0.3/sweatDB/sweatDB.py` & `sweatDB-2.0.4/sweatDB/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,77 @@
 import datetime
 import os
+version = "v2.0"
+e = os.path.isfile
+
 class actions :
-    version = "v2.1"
-    e = os.path.isfile
+    
+    # Create a database.
     
     def create(db):
         if e(db):
-            raise Exception("{db} already exists")
+            raise Exception(f"{db} already exists")
         else:
-            open(db).write(f"DATABASE NAME : {db} TIME CREATED : {datetime.datetime.utcnow()} CREATED WITH https://github.com/0xsweat/sweatDB {version}\n")
-            
-    def delete(ttd,db,item=''):
-        if e(name) != True:
-            return f"Database : {name} doesn't exist"
-        if ttd == "db":
+            open(db,'w').write(f"DATABASE NAME : {db} TIME CREATED : {datetime.datetime.utcnow()} CREATED WITH https://pypi.org/project/sweatDB/ {version}\n")
+    
+    # Delete an item or database.
+    
+    def delete(db,delete_type,item=''):
+        if e(db) != True:
+            return f"Database : {db} doesn't exist"
+        if delete_type == "db":
             os.remove(db)
         elif item == '':
             raise Exception('No item specified')
             a = open(db, 'r').read().split("\n")
             open(db, 'w').write("".join([f"{x}\n" for x in a if x.startswith(f'{item} ') == False])[:-1])
 
+    # Add an item to a database.
+
     def add(db,name,value):
         if e(db):
             open(db, 'a').write(f'{name} {value}\n')
         else:
             raise Exception(f'Database {db} not found')
 
+    # View ALL items, An item, item names, info, item count, and you can specify the limit with start && end.
+
     def view(db,option='all',item='',start=1,end=0):
+        option = option.lower()
         if e(db) != True:
             raise Exception(f'Database {db} not found')
         elif option == "all":
             c = open(db, 'r').read()
             if start < end and start > 0:
-                return ''.join(f'{x}\n' for x in c.split("\n")[start:end])
+                return ''.join(f'{x}\n' for x in c.split("\n")[start + 1:end + 2])
             else:
                 return c
         elif option == "item":
             b = open(db, 'r').read().split("\n")
+            output = ''
             for i in range(1,len(b)):
-                if b[i].startswith(f'{item} '):
-                    return(''.join([f'{x} ' for x in b[i].split(" ")[1:]])[:-1])
+                if b[i].startswith(f'{item}'):
+                    output += ''.join([f'{x} ' for x in b[i].split(" ")[1:]])[:-1] + "\n"
+            return output
             raise Exception(f'{item} not present in {db}')
         elif option == "items":
-            return(''.join([f'{x.split(" ")[0]}\n' for x in open(db, 'r').read().split('\n')[1:]])[:-2])
+            if start > end and start == 1:
+                return(''.join([f'{x.split(" ")[0]}\n' for x in open(db, 'r').read().split('\n')[1:]])[:-1])
+            else:
+                return(''.join([f'{x.split(" ")[0]}\n' for x in open(db, 'r').read().split('\n')[start + 1:end + 2]])[:-1])
         elif option == "info":
             return(open(db, 'r').read().split("\n")[0])
-        elif option == "itemcount":
+        elif option == "count":
             return(open(db, 'r').read().count("\n") - 1)
+                
+    # Edit an item in a database.
 
-    def edit(db,item,value):
+    def edit(db,item,value,t='value'):
         if e(db) != True:
             return f'Database {db} does not exist'
         b = open(db, 'r').read().split("\n")
         for x in range(len(b)):
-            if b[x].startswith(f'{item} '):
-                b[x] = f"{item} {newvalue}"
+            if b[x].startswith(f'{item}') and t=='value':
+                b[x] = f"{item} {value}"
+            elif b[x].startswith(f'{item}') and t!='value':
+                b[x] = f"{value} {''.join(f'{a} ' for a in [b[x].split(' ')[1:]])[:-1]}"
         open(db, 'w').write("".join([f"{x}\n" for x in b])[:-1])
```

